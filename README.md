# Exercise pose dataset

Pose data for classifying five bodyweight exercises by position. I used it while working on rep counting for [RapidRoutines](https://github.com/bgcalisthenics/rapidroutines).

There are 1,371 labeled poses. Each exercise has an up and a down position:

| Exercise | Labels |
| --- | --- |
| Jumping jacks | `jumping_jacks_up`, `jumping_jacks_down` |
| Pull-ups | `pullups_up`, `pullups_down` |
| Push-ups | `pushups_up`, `pushups_down` |
| Sit-ups | `situp_up`, `situp_down` |
| Squats | `squats_up`, `squats_down` |

## Files

All files share the `pose_id` column, so they can be joined row for row.

| File | Contents |
| --- | --- |
| `labels.csv` | the pose label for each `pose_id` |
| `landmarks.csv` | x, y and z for the 33 MediaPipe Pose landmarks |
| `angles.csv` | joint angles in degrees, such as elbow-shoulder-hip and hip-knee-ankle |
| `3d_distances.csv` | 3D distances between pairs of landmarks |
| `xyz_distances.csv` | the same distances split into x, y and z components |
