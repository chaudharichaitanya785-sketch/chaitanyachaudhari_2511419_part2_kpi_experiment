# Hypothesis Test Notes

## Metric Tested

Paid Conversion Rate

## Business Objective

Determine whether the new onboarding campaign (Treatment) significantly improves the paid conversion rate compared to the existing onboarding experience (Control).

## Null Hypothesis (H₀)

There is no significant difference in the paid conversion rate between the Control and Treatment groups.

H₀: p(Control) = p(Treatment)

## Alternative Hypothesis (H₁)

The Treatment group has a significantly higher paid conversion rate than the Control group.

H₁: p(Treatment) > p(Control)

## Test Used

Two-Proportion Z-Test

## Tail Type

One-tailed

## Significance Level (α)

0.05

## Test Inputs

Control Group:

* Users = 690
* Converted Users = 22
* Conversion Rate = 3.19%

Treatment Group:

* Users = 710
* Converted Users = 50
* Conversion Rate = 7.04%

## Test Results

Z Statistic = 3.264

P-value = 0.0011

## Decision Rule

If the p-value is less than 0.05, reject the null hypothesis.

Since 0.0011 < 0.05, the null hypothesis is rejected.

## Business Interpretation

The Treatment onboarding campaign produced a statistically significant improvement in paid conversion rate compared to the Control group. The observed improvement is unlikely to be due to random chance, providing strong evidence that the new onboarding experience is more effective at converting users into paying customers.
