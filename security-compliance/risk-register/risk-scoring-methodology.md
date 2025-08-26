# Risk Scoring Methodology

## Overview
This document defines the standardized approach for assessing, scoring, and prioritizing risks within the organization's risk management framework.

## Risk Assessment Framework

### Risk Formula
**Risk Score = Probability × Impact**

Where:
- **Probability**: Likelihood of the risk event occurring
- **Impact**: Magnitude of consequences if the risk materializes

## Probability Scale

### Probability Ratings (1-5 Scale)
| Rating | Level | Description | Frequency | Percentage |
|--------|-------|-------------|-----------|------------|
| 1 | Very Low | Extremely unlikely to occur | Once in 10+ years | 0-5% |
| 2 | Low | Unlikely to occur | Once in 5-10 years | 6-25% |
| 3 | Medium | Possible to occur | Once in 2-5 years | 26-50% |
| 4 | High | Likely to occur | Once per year | 51-75% |
| 5 | Very High | Almost certain to occur | Multiple times per year | 76-100% |

### Probability Assessment Factors
- **Historical Data**: Past occurrence frequency
- **Industry Trends**: Sector-specific threat landscape
- **Environmental Factors**: External conditions affecting likelihood
- **Control Effectiveness**: Current mitigation measures in place
- **Expert Judgment**: Subject matter expert assessment

## Impact Scale

### Impact Categories
1. **Financial Impact** - Direct monetary loss
2. **Operational Impact** - Business process disruption
3. **Reputational Impact** - Brand and customer trust damage
4. **Regulatory Impact** - Compliance violations and penalties
5. **Strategic Impact** - Long-term business objective effects

### Impact Ratings (1-5 Scale)
| Rating | Level | Financial | Operational | Reputational | Regulatory | Strategic |
|--------|-------|-----------|-------------|--------------|------------|-----------|
| 1 | Very Low | <$10K | <4 hours downtime | Minimal local impact | Minor compliance gap | Negligible effect |
| 2 | Low | $10K-$50K | 4-24 hours downtime | Local negative coverage | Regulatory notice | Minor delay |
| 3 | Medium | $50K-$250K | 1-3 days downtime | Regional coverage | Formal investigation | Moderate impact |
| 4 | High | $250K-$1M | 3-7 days downtime | National coverage | Significant penalties | Major setback |
| 5 | Critical | >$1M | >7 days downtime | International coverage | License revocation | Strategic failure |

### Impact Assessment Process
1. **Identify Affected Areas**: Determine which business functions would be impacted
2. **Quantify Consequences**: Estimate magnitude across all impact categories
3. **Consider Cascading Effects**: Assess secondary and tertiary impacts
4. **Apply Worst-Case Scenario**: Use maximum reasonable impact for scoring
5. **Document Assumptions**: Record basis for impact assessment

## Risk Score Matrix

### Risk Score Calculation
| Probability | Very Low (1) | Low (2) | Medium (3) | High (4) | Critical (5) |
|-------------|--------------|---------|------------|----------|--------------|
| **Very High (5)** | 5 | 10 | 15 | 20 | 25 |
| **High (4)** | 4 | 8 | 12 | 16 | 20 |
| **Medium (3)** | 3 | 6 | 9 | 12 | 15 |
| **Low (2)** | 2 | 4 | 6 | 8 | 10 |
| **Very Low (1)** | 1 | 2 | 3 | 4 | 5 |

### Risk Level Classification
| Risk Score | Risk Level | Color Code | Management Action Required |
|------------|------------|------------|---------------------------|
| 20-25 | Extreme | Red | Immediate executive attention |
| 15-19 | High | Orange | Senior management oversight |
| 10-14 | Medium | Yellow | Management monitoring |
| 5-9 | Low | Green | Routine monitoring |
| 1-4 | Very Low | Blue | Accept or minimal controls |

## Risk Response Strategies

### Response Options
1. **Avoid** - Eliminate the risk by changing business processes
2. **Mitigate** - Reduce probability or impact through controls
3. **Transfer** - Shift risk to third parties (insurance, outsourcing)
4. **Accept** - Acknowledge risk and monitor without additional controls

### Response Selection Criteria
| Risk Level | Primary Response | Secondary Options | Approval Required |
|------------|------------------|-------------------|-------------------|
| Extreme | Avoid/Mitigate | Transfer | Board/CEO |
| High | Mitigate | Avoid/Transfer | Executive Team |
| Medium | Mitigate/Transfer | Accept | Senior Management |
| Low | Accept/Mitigate | Transfer | Department Manager |
| Very Low | Accept | Mitigate | Risk Owner |

## Control Effectiveness Assessment

### Control Maturity Levels
| Level | Description | Effectiveness Rating | Risk Reduction |
|-------|-------------|---------------------|----------------|
| 1 | Ad-hoc | Ineffective | 0-20% |
| 2 | Repeatable | Partially Effective | 21-40% |
| 3 | Defined | Effective | 41-60% |
| 4 | Managed | Highly Effective | 61-80% |
| 5 | Optimized | Very Highly Effective | 81-95% |

### Residual Risk Calculation
```
Residual Risk = Inherent Risk × (1 - Control Effectiveness)

Example:
Inherent Risk Score: 15 (High)
Control Effectiveness: 60% (Effective)
Residual Risk = 15 × (1 - 0.60) = 6 (Low)
```

## Risk Assessment Process

### Step 1: Risk Identification
- **Brainstorming Sessions** - Cross-functional team workshops
- **Historical Analysis** - Review past incidents and near-misses
- **Industry Research** - Analyze sector-specific threats
- **Regulatory Review** - Assess compliance requirements
- **Stakeholder Input** - Gather insights from business units

### Step 2: Risk Analysis
```python
# Risk scoring calculation example
def calculate_risk_score(probability, impact):
    """
    Calculate risk score based on probability and impact
    """
    risk_score = probability * impact
    
    if risk_score >= 20:
        risk_level = "Extreme"
    elif risk_score >= 15:
        risk_level = "High"
    elif risk_score >= 10:
        risk_level = "Medium"
    elif risk_score >= 5:
        risk_level = "Low"
    else:
        risk_level = "Very Low"
    
    return risk_score, risk_level
```

### Step 3: Risk Evaluation
- **Risk Tolerance Assessment** - Compare against organizational appetite
- **Cost-Benefit Analysis** - Evaluate mitigation investment vs. risk reduction
- **Regulatory Requirements** - Ensure compliance obligations are met
- **Stakeholder Impact** - Consider effects on customers, partners, employees

### Step 4: Risk Treatment
- **Develop Action Plans** - Create specific mitigation strategies
- **Assign Ownership** - Designate responsible parties
- **Set Timelines** - Establish implementation schedules
- **Allocate Resources** - Ensure adequate funding and personnel

## Quality Assurance

### Risk Assessment Review Process
1. **Peer Review** - Independent validation by risk management team
2. **Subject Matter Expert Review** - Technical validation by domain experts
3. **Management Review** - Business validation by senior leadership
4. **Board Oversight** - Governance review of extreme and high risks

### Common Assessment Errors
- **Probability Overestimation** - Focusing on worst-case scenarios
- **Impact Underestimation** - Failing to consider cascading effects
- **Control Overconfidence** - Overrating control effectiveness
- **Bias Influence** - Personal experience skewing assessment
- **Incomplete Analysis** - Missing secondary or tertiary impacts

## Monitoring and Review

### Review Frequency
| Risk Level | Review Frequency | Trigger Events |
|------------|------------------|----------------|
| Extreme | Monthly | Any material change |
| High | Quarterly | Significant changes |
| Medium | Semi-annually | Annual or major changes |
| Low | Annually | Major business changes |
| Very Low | Bi-annually | Significant external changes |

### Key Risk Indicators (KRIs)
- **Cybersecurity**: Number of security incidents, vulnerability counts
- **Operational**: System downtime, change failure rates
- **Compliance**: Audit findings, regulatory notices
- **Financial**: Budget variances, cost overruns
- **Strategic**: Project delays, market changes

### Risk Reporting
- **Executive Dashboard** - High-level risk metrics and trends
- **Risk Register Updates** - Detailed risk status and changes
- **Incident Reports** - Risk materialization and lessons learned
- **Trend Analysis** - Risk landscape evolution and emerging threats