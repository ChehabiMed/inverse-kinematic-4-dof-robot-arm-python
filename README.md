# 4 dof Robotic Arm Kinematics Visualization


  ![Robotic Arm](notebook_img.png)

The image represent four links starting with the base link in Red to the end effector in Cyan, and also a projection point on the 2D plane.



## Files

- `IK_4DOF.ipynb`: Main notebook script to calculate the forward and inverse kinematics and visualize the robotic arm.


## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/ChehabiMed/inverse-kinematic-4-dof-robot-arm-python.git
    cd inverse-kinematic-4-dof-robot-arm-python
    ```

2. Open Jupyter Notebook and navigate to the repository directory.

3. Open and run `IK_4DOF.ipynb` to calculate the forward and inverse kinematics and visualize the robotic arm.

## IK_4DOF.ipynb

This notebook script performs the following tasks:

### Initialization:
- Defines the lengths of the arm segments and the target end-effector position.

### DH Method:
- Defines the function `DHmethode` to create the Denavit-Hartenberg (DH) transformation matrix for each joint.

### Joint Angle Calculation:
- Defines the function `calculate_joint_angles` to compute the joint angles required to reach the target end-effector position using inverse kinematics.

### Transformation Matrix:
- Calculates the transformation matrices for each joint.
- Multiplies the matrices to get the overall transformation matrix from the base to the end-effector.
- Prints the final transformation matrix.

### 3D Visualization:
- Computes the positions of the end-effector and joints.
- Plots the robotic arm in 3D space.

## DHmethode Function

This function creates the DH transformation matrix for a given joint. It takes the following parameters:

- `a`: Link length.
- `alpha`: Link twist.
- `d`: Link offset.
- `theta`: Joint angle.

The function returns the 4x4 DH transformation matrix.

To see the robotic arm in action, run the `IK_4DOF.ipynb`. The notebook will output the transformation matrix and plot the arm in 3D space.

## License

This project is licensed under the MIT License.
