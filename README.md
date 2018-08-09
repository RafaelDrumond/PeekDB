# PeekDB

If you want to use this data-set please reference it as:
```
@inproceedings{drumond2018peek,
  title={PEEK-An LSTM Recurrent Network for Motion Classification from Sparse Data.},
  author={Drumond, Rafael Rego and Marques, Bruno AD and Vasconcelos, Cristina Nader and Clua, Esteban},
  booktitle={VISIGRAPP (1: GRAPP)},
  pages={215--222},
  year={2018}
}
```
## Data
Each motion sequence is located on the motion folder. The actors have been anonimized to a number. Each files contains a sequence of the actions. Each line is one time step. The first number is the time-stamp followed by 11 values for the left arm and 11 for the right arm respectively. Each of these 11 Values are (in order): the quaternion [x,y,z,w] representing arm orientation (4 first values), euler angles of the arm (3 middle values), and a quaternion for angular speed of the arm (4 last values). The last 7 numbers after "|class" are just an encoding for the class an can be ignored since all motion frames are from the same class in the same file.

## Motion types
* Running
* Walking
* Crouching (a person crouching and standing at the same time)
* Swing (A person swinging an weapon)
* Idle (a person not doing nothing special, standing, maybe checking his/her phone, but not moving around)
