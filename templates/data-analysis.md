# Data Analysis Prompt Template

## Purpose
Analyze datasets and extract actionable insights.

## Template

\`\`\`
Analyze the following dataset and provide insights:

**Data:**
[Paste data or describe dataset]

**Analysis Required:**
1. Summary statistics (mean, median, mode, std dev)
2. Key trends or patterns
3. Anomalies or outliers
4. Correlations between variables
5. Actionable recommendations

**Output Format:**
- JSON structure with clear sections
- Include confidence levels for insights
- Prioritize by business impact

**Context:**
[What decisions will this analysis inform?]
\`\`\`

## Example Usage

**Input:**
\`\`\`
Analyze the following sales data:

Data:
Month,Sales,Marketing_Spend,Customer_Count
Jan,50000,5000,120
Feb,45000,4500,110
Mar,65000,8000,150
Apr,70000,8500,165
May,55000,6000,130

Analysis Required:
1. Summary statistics
2. Relationship between marketing spend and sales
3. Customer acquisition trends
4. Month-over-month growth patterns
5. Budget recommendations

Output Format: JSON

Context: Planning Q3 marketing budget allocation
\`\`\`