# LOGISTIC REGRESSION (Simple Rule)
features = ["study_hours", "attendance", "previous_grades"]
# Makes sense: More study = higher chance to pass (simple relationship)

# RANDOM FOREST (Complex Rules)
features = ["study_hours", "attendance", "sleep_hours", "breakfast", 
            "stress_level", "class_participation", "homework_done", 
            "tutor_help", "part_time_job", "sports_practice"]
# Better when: Many factors combine in unique ways
# "Studied little but slept well, had breakfast, and did homework" - complex pattern!

Choose LogisticRegression when:
python
✅ Data is small (< 1000 samples)
✅ Relationship is simple and straight
✅ You need fast predictions
✅ You want to understand WHY (feature importance is clear)
✅ Features are not strongly connected to each other

# Example:
X = [[30, 1], [40, 1], [50, 0]]  # [age, smokes?]
y = [0, 1, 1]  # has disease?
# Simple: Age + smoking → disease risk
Choose RandomForestClassifier when:
python
✅ Data is large (> 1000 samples)
✅ Relationship is complex and twisty
✅ You have many features (10+)
✅ You don't care HOW it decides, just accuracy
✅ Features interact in complex ways

# Example:
X = [[30, 1, 0, 5, 100], [40, 0, 1, 2, 150]]  # Many features!
y = [0, 1]  # will buy product?
# Complex: Age + income + browsing + previous purchases + time of day