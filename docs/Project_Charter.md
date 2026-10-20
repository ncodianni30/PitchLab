
# PitchLab — Project Charter

## Project Purpose
Develop a data-driven pitcher development optimization system that identifies potential improvements for struggling pitchers through historical pitching data.

The software will analyze relationships between mechanics, pitch characteristics, and performance to identify realistic and individualized development opportunities.

## Primary Research Question
Can historical pitching data be used to identify effective combinations of pitching characteristics and determine realistic adjustments that may improve an individual pitcher's performance?

## Model Architecture

### Model 1: Pitching Relationships
Identify how pitching mechanics and pitch characteristics interact and change together.

Variables of interest include:
- Arm angle
- Release position
- Release extension
- Velocity
- Spin rate and spin axis
- Horizontal and vertical movement
- Pitch type

### Model 2: Successful Pitching Profiles
Identify multiple combinations of pitching characteristics associated with successful outcomes.

Recognize that pitchers can achieve success through different combinations of mechanics, pitch characteristics, and arsenal construction.

### Model 3: Individualized Development Pathways
Determine which successful pitching profiles are most realistically attainable for individual pitchers.

Generate potential adjustments and combinations while considering feasibility, uncertainty, and tradeoffs.

## Initial Data Sources
- MLB Statcast / Baseball Savant
- pybaseball (Python)

## Planned Development Order
1. Data collection and exploration
2. Relationships model
3. Successful profiles model
4. Development pathways model
5. Historical validation
6. Interactive application and visualization

## Project Principles
- No universal ideal pitching profile
- Pitching characteristics are interconnected
- Recommendations must be individualized
- Historical correlations do not necessarily imply causation
- Model predictions must be validated on unseen data
- Physical feasibility and pitcher safety must be considered

## Long-Term Goal
Develop a functional research and decision-support tool that could assist professional baseball player development departments.
