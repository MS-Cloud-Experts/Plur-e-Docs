### API Documentation: Route Optimization

#### Overview
The `Route Optimization` API provides an interface to generate optimized delivery routes for the Plur-e WMS system. It offers two optimization strategies: full optimization (including distances and times) and priority-based optimization (based on customer priorities and order values). The API processes the selected sales orders and returns an optimized delivery sequence considering various factors like customer priority, order value, and delivery logistics.

#### Request Structure
```json
{
  "ProcessMethod": "OptimizeRoute",
  "Parameters": [
    {
      "strategy": "full",
      "prompt": "Generate optimized route for pending deliveries"
    }
  ]
}
```

#### Parameters
- **strategy**: String specifying the optimization type. Valid values:
  - `full`: Complete optimization considering distances and delivery times
  - `priority`: Priority-based optimization focusing on customer priority and order value
- **prompt**: String containing the route optimization request

#### Example Request
```json
{
  "ProcessMethod": "OptimizeRoute",
  "Parameters": [
    {
      "strategy": "full",
      "prompt": "Optimize delivery route for Madrid area shipments"
    }
  ]
}
```

#### Example Response
```json
{
  "success": true,
  "routes": [
    {
      "orderId": "SO-001",
      "customerNo": "C00123",
      "customerName": "Customer A",
      "deliverySequence": 1,
      "customerPriority": "VIP",
      "orderValue": 1500.00,
      "packageSize": "Large",
      "productWeight": 25.5,
      "deliveryDistance": 15.2,
      "estimatedDeliveryTime": "2.5",
      "details": "First delivery of the route"
    }
  ]
}
```

#### Response Fields
- **success**: Boolean indicating whether the route optimization was successful
- **routes**: Array of optimized delivery routes containing:
  - **orderId**: Sales order identifier
  - **customerNo**: Customer number
  - **customerName**: Customer name
  - **deliverySequence**: Optimized delivery order
  - **customerPriority**: Customer priority level
  - **orderValue**: Total order value
  - **packageSize**: Size classification of the package
  - **productWeight**: Total weight of the order
  - **deliveryDistance**: Distance in kilometers (full optimization only)
  - **estimatedDeliveryTime**: Estimated delivery time in hours (full optimization only)
  - **details**: Additional route information

#### Error Response
```json
{
  "success": false,
  "error": "Invalid optimization strategy"
}
```

#### Common Error Messages
- **"Strategy and prompt are required"**: Missing required parameters
- **"Invalid optimization strategy"**: Invalid strategy value
- **"No sales orders selected"**: No pending orders found for optimization

#### Optimization Strategies

##### Full Optimization
Considers:
- Customer priority levels (VIP, regular)
- Delivery distances and times
- Order values
- Package sizes and weights

##### Priority-Based Optimization
Considers:
- Customer priority levels (VIP, regular)
- Order values
- Package sizes and weights
- Does not include distance calculations

#### Technical Details
- Uses Bing Maps API for distance calculations in full optimization
- Caches route distances for 30 days
- Maximum supported stops per route: Unlimited
- Supports multiple package sizes: Small, Medium, Large
- Integrates with existing WMS shipment data

#### Security Notes
- Requires proper authentication
- Distance calculations are cached securely
- Customer data is handled according to privacy policies
- Route optimizations are logged for auditing

#### Best Practices
1. **Strategy Selection**:
   - Use `full` when delivery timing is critical
   - Use `priority` for simpler priority-based sequencing
2. **Order Preparation**:
   - Ensure all orders are marked as picked
   - Verify customer addresses are complete
   - Check package dimensions and weights are updated
3. **Optimization Timing**:
   - Run optimizations close to delivery time
   - Consider running multiple scenarios

#### Example Use Cases
1. **Daily Route Planning**: "Optimize tomorrow's delivery routes for all pending orders"
2. **Priority Deliveries**: "Create a route prioritizing VIP customer deliveries"
3. **Zone-Based Delivery**: "Optimize routes for north zone deliveries"
4. **Mixed Load Planning**: "Plan route for mixed package sizes with priority customers"

#### Usage Guidelines
1. Ensure all orders are in "Picked" status before optimization
2. Verify customer addresses are complete for accurate distance calculations
3. Keep package dimensions and weights updated for better optimization
4. Consider time windows and delivery constraints in the optimization request

#### Summary
The Route Optimization API provides a powerful tool for optimizing delivery routes in the Plur-e WMS system. It offers flexible optimization strategies to meet different business needs, from simple priority-based sequencing to complex distance-based routing with time estimations.