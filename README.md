## Gesture Recognition

### Problem Statement:

You are working as a data scientist at a home electronics company that manufactures state-of-the-art smart televisions. The objective is to develop a cool feature for the smart TV that can recognize five different gestures performed by the user, enabling them to control the TV without using a remote.

The gestures are continuously monitored by the webcam mounted on the TV, and each gesture corresponds to a specific command:

- Thumbs up: Increase the volume 👍🔊
- Thumbs down: Decrease the volume 👎🔉
- Left swipe: 'Jump' backward 10 seconds ⬅️⏪
- Right swipe: 'Jump' forward 10 seconds ➡️⏩
- Stop: Pause the movie 🤚⏸️

The training data consists of several hundred videos categorized into one of the five classes. Each video, typically 2-3 seconds long, is divided into a sequence of 30 frames (images). These videos have been recorded by various people performing one of the five gestures in front of a webcam, similar to what the smart TV will use.

## Conclusion

### Top Models:

- **Model 10 using Conv3D**
  - Validation loss = 2.31314
  - Validation accuracy = 79%
  - Size = 7.38 MB
  - Total params = 1,933,765

- **RNN + CNN Model 2 using GRU**
  - Validation loss = 0.63840
  - Validation accuracy = 81%
  - Size = 5.04 MB
  - Total params = 1,320,037

### Results Table:

| Ground Truth   | Predicted Value |
|----------------|-----------------|
| Thumbs_Up      | Thumbs_Up       |
| Left_Swipe     | Left_Swipe      |
| Thumbs_Up      | Thumbs_Up       |
| Left_Swipe     | Left_Swipe      |
| Thumbs_Up      | Thumbs_Up       |
| Thumbs_Down    | Thumbs_Down     |
| Thumbs_Up      | Thumbs_Up       |
| Stop           | Right_Swipe     |
| Right_Swipe    | Stop            |
| Left_Swipe     | Left_Swipe      |
| Right_Swipe    | Right_Swipe     |
| Thumbs_Down    | Thumbs_Down     |
| Right_Swipe    | Right_Swipe     |
| Stop           | Stop            |
| Stop           | Stop            |
| Thumbs_Down    | Thumbs_Down     |
| Thumbs_Down    | Thumbs_Down     |
| Right_Swipe    | Right_Swipe     |
| Right_Swipe    | Right_Swipe     |
| Right_Swipe    | Right_Swipe     |
| Thumbs_Down    | Thumbs_Down     |
| Thumbs_Up      | Thumbs_Up       |
| Thumbs_Up      | Thumbs_Up       |
| Stop           | Stop            |
| Stop           | Stop            |
| Left_Swipe     | Left_Swipe      |
| Left_Swipe     | Left_Swipe      |
| Stop           | Left_Swipe      |
| Thumbs_Down    | Thumbs_Down     |
| Right_Swipe    | Right_Swipe     |

Accuracy: 90.00%
