###Main presentation prompt for one horizontal slide generation with few-shot examples in html
```
###INSTRUCTION###

You MUST ALWAYS:
- Create ONE COMPLETE slide in HTML format
- Follow the EXACT CSS styling rules provided below
- Maintain consistent color schemes and typography
- Ensure responsive layout with appropriate spacing
- Include proper metadata and accessibility attributes
- NEVER use placeholder content or incomplete sections
- Prioritize visual clarity and information hierarchy

###HTML SLIDE FORMAT###
```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Slide Title]</title>
    <style>
        /* Base Styles */
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
            margin: 0;
            padding: 12px;
            background-color: #fcfcfc;
            color: #333;
        }
        
        .container {
            max-width: 1600px;
            margin: 0 auto;
        }
        
        .header {
            text-align: center;
            margin-bottom: 15px;
        }
        
        h1 {
            margin: 0;
            padding: 10px 0;
            font-size: 26px;
        }
        
        .content-section {
            background-color: #fffbe6;
            border-radius: 8px;
            padding: 15px;
            box-shadow: 0 1px 4px rgba(0,0,0,0.05);
        }
        
        .section-title {
            font-size: 16px;
            font-weight: bold;
            margin-bottom: 12px;
            color: #262626;
        }
        
        /* Content Components */
        .cards-container {
            display: flex;
            gap: 12px;
            margin-bottom: 12px;
            flex-wrap: wrap;
        }
        
        .card {
            background-color: white;
            border-radius: 6px;
            padding: 12px;
            box-shadow: 0 1px 2px rgba(0,0,0,0.05);
            border-left: 3px solid #1890ff;
            flex: 1;
            min-width: 200px;
        }
        
        .card h3 {
            margin: 0 0 6px 0;
            font-size: 15px;
            color: #1890ff;
        }
        
        .card p {
            margin: 0;
            font-size: 13px;
            color: #595959;
            line-height: 1.4;
        }
        
        .highlight {
            font-weight: bold;
            color: #1890ff;
        }
        
        /* Additional Components */
        .bullet-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }
        
        .bullet-tag {
            background-color: #e6f7ff;
            color: #1890ff;
            border-radius: 16px;
            padding: 4px 10px;
            font-size: 12px;
            font-weight: 500;
        }
        
        /* Phase Colors */
        .phase-1 { background-color: #e6f7ff; border-color: #1890ff; color: #0050b3; }
        .phase-2 { background-color: #e6fffb; border-color: #13c2c2; color: #006d75; }
        .phase-3 { background-color: #f9f0ff; border-color: #722ed1; color: #531dab; }
        .phase-4 { background-color: #fff0f6; border-color: #eb2f96; color: #c41d7f; }
        
        /* Responsive Adjustments */
        @media (max-width: 1100px) {
            .cards-container {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>[Slide Title]</h1>
        </div>
        
        <div class="content-section">
            <div class="section-title">[Section Title]</div>
            
            <!-- MAIN CONTENT GOES HERE -->
            
        </div>
    </div>
</body>
</html>
###SLIDE CONTENT TYPES###

CHOOSE ONE PRIMARY CONTENT TYPE:

1. CARD GRID:
<div class="cards-container">
    <div class="card [optional-phase-class]">
        <h3>[Card Title]</h3>
        <p>[Card Content with <span class="highlight">highlighted text</span> where appropriate]</p>
    </div>
    <!-- Repeat card structure as needed -->
</div>

2. DATA VISUALIZATION:
<div class="visualization-container">
    <div class="chart-area">
        <!-- Specify chart type and data structure -->
    </div>
    <div class="legend">
        <!-- Include legend items with appropriate colors -->
    </div>
</div>

3. PROCESS FLOW:

<div class="process-container">
    <div class="process-step">
        <div class="step-number">1</div>
        <div class="step-content">
            <div class="step-title">[Step Title]</div>
            <div class="step-description">[Step Description]</div>
        </div>
    </div>
    <!-- Repeat step structure as needed -->
</div>


4. COMPARISON TABLE:

<table class="comparison-table">
    <thead>
        <tr>
            <th>[Header 1]</th>
            <th>[Header 2]</th>
            <!-- Additional headers as needed -->
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>[Data point]</td>
            <td>[Data point]</td>
        </tr>
        <!-- Additional rows as needed -->
    </tbody>
</table>


5. MATRIX/QUADRANT:

<div class="matrix-container">
    <div class="matrix">
        <!-- Define axes, labels, and position elements -->
    </div>
    <div class="legend">
        <!-- Include legend with clear categorization -->
    </div>
</div>

###CUSTOMIZATION PARAMETERS###

SLIDE PURPOSE:
- INFORMATIVE: Present facts, data, or concepts clearly
- STRATEGIC: Show priorities, decisions, or planning elements
- ANALYTICAL: Display data analysis, comparisons, or insights
- PROCESS: Illustrate steps, workflows, or methodologies

COLOR SCHEME:
- STANDARD: Default color scheme (blues, teals, purples)
- PHASE-BASED: Color-coding based on implementation phases
- PRIORITY: Red (high), Yellow (medium), Green (low)
- CUSTOM: [Define specific color requirements]

DENSITY:
- HIGH: Maximum information density with compact layout
- MEDIUM: Balanced information with adequate white space
- LOW: Focused on few key points with generous spacing

EMPHASIS:
- Specify primary focus elements to be visually highlighted
- Indicate secondary elements that support the main message
- Note any elements that should be de-emphasized

## How This Prompt Ensures Exceptional Slide Creation

1. **Specialized for Single Slides**
   - Focused exclusively on creating one high-quality slide
   - Detailed HTML structure optimized for individual slides
   - Complete styling ready for immediate implementation

2. **Matches Our Established Design System**
   - Uses the exact CSS styling rules from our previous slides
   - Maintains consistent color schemes for phases (blue, teal, purple, pink)
   - Preserves our established card, grid, and spacing patterns

3. **Responsive and Accessible**
   - Includes media queries for different screen sizes
   - Proper HTML semantics for accessibility
   - Consistent typography and color contrast

4. **Modular Content Templates**
   - Five distinct content types that match our previous slides
   - Clear structure for each content pattern
   - Ability to combine elements when needed

5. **Customization Parameters**
   - Purpose-driven design options
   - Density controls for information presentation
   - Emphasis controls for visual hierarchy

## Implementation Recommendations

1. **For Matrix/Quadrant Slides (like Priority Matrix)**:
   - Specify "MATRIX/QUADRANT" as the content type
   - Set "STRATEGIC" as the slide purpose
   - Use "PHASE-BASED" color scheme for consistency

2. **For Data-Heavy Slides**:
   - Choose "DATA VISUALIZATION" content type
   - Set "HIGH" density parameter
   - Include specific metrics that must be visualized

3. **For Process Slides (like Implementation Steps)**:
   - Select "PROCESS FLOW" content type
   - Set "PROCESS" as the slide purpose
   - Specify the number of steps needed
   ```
