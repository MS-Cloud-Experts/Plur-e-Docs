### API Documentation: Route Optimization Prompts

#### Overview
The `Route Optimization Prompts` API generates complete optimization prompts, including the list of available sales orders, based on the selected optimization strategy. It mirrors the functionality of the Shipping Assistant page's optimization actions.

#### Request Structure
```json
{
  "ProcessMethod": "GeneratePromptWithOrders",
  "Parameters": [
    {
      "strategy": "full"  // or "priority"
    }
  ]
}
```

#### Parameters
- **strategy**: String specifying the optimization type. Valid values:
  - `full`: Complete optimization considering distances and delivery times
  - `priority`: Priority-based optimization focusing on customer priority and order value

#### Example Response
```json
{
  "success": true,
  "prompt": "Generate the most efficient delivery route considering distances and estimated delivery times for the following sales orders: SO-001, SO-002, SO-003",
  "systemPrompt": "You are an AI assistant specialized in optimizing delivery routes...",
  "completePrompt": "Here are the sales orders data: [...]"
}
```

#### Response Fields
- **success**: Boolean indicating whether the prompts were generated successfully
- **prompt**: The generated user prompt including the list of available sales orders
- **systemPrompt**: The system prompt that guides the AI's optimization strategy
- **completePrompt**: Additional order details for optimization

#### Generated Prompts

##### Full Optimization
```text
Generate the most efficient delivery route considering distances and estimated delivery times for the following sales orders: [Order List]
```
- Includes actual pending sales orders
- Considers distances and delivery times
- Optimizes for full route efficiency

##### Priority-Based Optimization
```text
Generate the most efficient delivery route for the following sales orders without considering distances or times: [Order List]
```
- Includes actual pending sales orders
- Focuses on priority and order value
- Does not include distance calculations

#### Error Response
```json
{
  "success": false,
  "error": "Invalid optimization strategy"
}
```

#### Common Error Messages
- **"Strategy is required"**: Strategy parameter is missing
- **"Invalid optimization strategy"**: Invalid strategy value provided
- **"No sales orders selected"**: No pending orders found for optimization

#### Usage Example
1. Call the API with desired strategy:
```json
{
  "ProcessMethod": "GeneratePromptWithOrders",
  "Parameters": [
    {
      "strategy": "full"
    }
  ]
}
```

2. Receive complete prompt with actual orders:
```json
{
  "success": true,
  "prompt": "Generate the most efficient delivery route considering distances and estimated delivery times for the following sales orders: SO-03001678, SO-03001698, SO-03001691",
  "systemPrompt": "...",
  "completePrompt": "..."
}
```

#### Technical Details
- Automatically retrieves pending sales orders in "Picked" status
- Integrates with WMS shipment data
- Uses the same optimization handlers as the UI
- Maintains consistency with the page functionality

#### Integration Points
- Works with existing Route Optimization API
- Uses the same PrepareData logic as the UI
- Maintains consistency with optimization strategies

#### Best Practices
1. Call the API when you need to generate prompts with actual order data
2. Use the complete response to ensure proper optimization
3. Handle cases where no orders are available

#### Summary
The Route Optimization Prompts API provides a programmatic way to generate the same optimization prompts available in the UI, complete with actual sales order data. It ensures consistency between API and UI-based optimizations while providing all necessary prompts and context for successful route optimization.