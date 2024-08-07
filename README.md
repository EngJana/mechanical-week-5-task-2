# mechanical-week-5-task-2

Smart Methods Internship - Week 5 Task 2: Plenty Gears

This project demonstrates how to create and animate mechanical gears in Blender.

## Gear Specifications

small gears:
- **Gear A**: 20 teeth, radius 1 m
- **Gear B**: 20 teeth, radius 1 m
- **Gear C**: 20 teeth, radius 1 m
big gear:
- **Gear D**: 60 teeth, radius 3 m

## Setup Instructions

### 1. Add Gears

1. Open Blender.
2. Go to **Edit > Preferences > Add-ons**.
3. Enable **Add Mesh: Extra Objects**.
4. In the 3D Viewport, navigate to **Add > Mesh > Gears** to add the gears.
5. Set the number of teeth for each gear as specified.

### 2. Modify the Large Gear

1. Enter **Edit Mode**.
2. Select the lower inside edge of the gear.
3. Use the Scale tool, press `Alt`, then drag towards the center to close the gear.
4. Repeat for the upper edge.
5. Add a cylinder matching the gear size.
6. Select the cylinder, add a **Boolean** modifier.
7. In the Boolean settings, select the large gear.
8. Apply the Boolean modifier and delete the original large gear.

### 3. Position Gears

1. Use the Move and Rotate tools to interlock the gear teeth properly.
2. Ensure all gears are aligned for smooth animation.

### 4. Gear Rotation Setup

#### Small Gears:

1. Select a small gear.
2. Go to **Constraints**.
3. Add **Copy Rotation**.
4. Select the adjacent small gear in the object box.
5. Set the rotation axis (e.g., Z-axis) and invert it for opposite direction.
6. Repeat for the other small gear, ensuring the middle gear drives the others.

#### Large Gear:

1. Select the large gear.
2. Go to **Constraints**.
3. Add **Transformation**.
4. Select a nearby small gear in the object box.
5. Check **Extrapolate**.
6. Set **Map From** rotation max Z to 360 degrees. (meaning when the small gear have a full rotation …)
7. Set **Map To** rotation max Z to 120 degrees (… the big gear will have 1/3 rotation)

### 5. Set Keyframes for Animation

1. Set the timeline frame to 0.
2. Press `A` to select all gears.
3. Press `I` to insert keyframes at the starting position.
4. Move the timeline to frame 60.
5. Rotate the middle gear.
6. Press `A` then `I` to insert keyframes at the new position.
7. Continue until Gear D completes a full rotation.

  <img width="327" alt="Screenshot 2024-08-07 220759" src="https://github.com/user-attachments/assets/dffc2b31-13a4-4e7f-b64e-e33096584e89">
 
