# Unreal_VR_Pawn-flying-camera_snapshot-etc
A sample VR pawn project in UE4 that allows the user to take handheld camera snapshots, fly freely and teleport. More features coming soon. It is being built on an oculus rift, but should in theory also work on a vive. 
Demo video: https://www.youtube.com/watch?v=tYhlMPEB7_0&t=22s

Open the project and hit play in VR. Currently there is not mouse and keyboard version.
Both hands now can be any of nine control modes. Press button 1 (A or X on an oculus touch) to switch modes. When you switch modes you will drop all held items. 
  Fly Mode: Text will appear directly above your hand
    Trigger - fly in the direction the controller is facing. Pressure changes speed
    Thumbstick up/down - change speed of flight
    thumbstick click and left/right - rotate camera in 45 degree incriments
    grip trigger - grab object.
  Teleport Mode:
    Trigger Pressed - starts teleportation. hold down and point where you would like to go
    Trigger Released - teleport to selected location
    Thumbstick - rotates the view on teleport landing
    Thumbstick click - switches to a mode where the thumbstick changes your teleport distance
    grip trigger - grab object
  Grab Mode:
    Grip trigger -  grab object
    Coming soon: thumbstick controls rotation of object and distance from hand
  Snapshot Mode: Your hand will turn into a camera viewport. 
    Trigger - take snapshot
    Thumb left/right - zoom in and out
    Thumb down+click in - take a snapshot of the HMD view
  Laser pointer mode:
    Thumb up+click - change units
    Thumb down+click - hide distance to object display
    Trigger - place one of two measurement points
  Beacon teleport mode:
    requires teleport beacons to be placed. They are in the VR controller folder and are invisible during the game by default. Any              number of beacons is supported
    Thumb up+click - teleport to next beacon
    Thumb down+click - teleport to last beacon
    Button 2 (B or Y on an oculus) place new beacon. This beacon will be destroyed on exiting gameplay, so if you would like to keep it,        alt tab to the editor, select the beacon, copy, exit game mode, paste
  Flashlight mode:
    Trigger - turn on and off
    thumbstick up/down - change brightness
    thumbstick left/right - change beam size
  Empty mode:
    No hand or tool visible
    

Snapshots are saved to the {root}/Unreal/Snapshots where root is which drive you have the project downloaded to as HDR files. Photoshop will open them. 


  make the camera snapshot tool vibrate on a capture
  add stabalization options to the handheld camera
  add a video camera
  Create a mouse and keyboard version that autodetects the headset being off/not in use
  in grab mode add functionality to move/rotate objects using the thumbstick
  add a laser select mode that allows the user to select an item and use position/rotation/scale gizmos to edit it, and change material/etc
  change the mode switch from a button cycle to a radial menu
  add a spawn objects menu
  add a menu function to change world scale in game
  writeup master materials functionality in development
  add a function to save object changes without the copy and paste nonsense
