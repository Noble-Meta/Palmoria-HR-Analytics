# Palmoria HR Analytics – Insights Notes

This document captures key findings, interpretations, and important notes generated during the analysis of Palmoria Group's HR data using Power BI.

---

## Gender Distribution

- **Observation:** Some departments have a significant gender imbalance. <br>
For example **Product Management** has noticeably more male employees than female.
- **Action Point:** Consider revisiting recruitment strategies in departments with low female representation.

---

## Performance Ratings by Gender

- **Observation:** Female employees in the Services and Legal departments had slightly higher average ratings.
- **Note:** Rating data was converted from text to numerical scores using a DAX column.

---

## Gender Pay Gap

- **Observation:** Gender pay disparities are prominent in departments like Business Development and Support.
- **Example:** In Business Development, males earn an average of $82,016 while females earn $74,627.
- **Action Point:** Recommend salary audits in flagged departments.

---

## Salary Band Compliance

- **Observation:** 654 employees earn below the regulatory minimum salary of $90,000.
- **Region Most Affected:** Kaduna.
- **Action Point:** Immediate salary structure review is advised to avoid regulatory risks.

---

## Bonus Allocation

- **Methodology:** Bonus computed based on department + rating score using merged lookup logic.
- **Total Bonus Payout:** $2.2M
- **Note:** Bonus percentages were defined in a separate bonus rules table and applied via DAX lookup.

---

## Other Notes

- Null or missing departments and salaries were removed during Power Query cleaning.
- Undisclosed gender was assigned a generic category "Undisclosed" for fairness in visuals.
- Data relationships were created using `DeptRatingKey` for accurate bonus mapping.

---

## Next Steps

- Implement HR interventions in flagged regions and departments.
- Automate future salary audits using Power BI alerts or Excel pivot models.
- Develop a KPI dashboard for ongoing HR monitoring.
