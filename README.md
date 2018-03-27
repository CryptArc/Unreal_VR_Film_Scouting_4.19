# Unreal_VR_Pawn-flying-camera_snapshot-etc
A sample VR pawn project in UE4 that allows the user to take handheld camera snapshots, fly freely and teleport. More features coming soon. It is being built on an oculus rift, but should in theory also work on a vive. Eventually I would like to figure out how to incorperate some of this functionality into the VR editor. 

Open the project and hit play in VR. Currently there is not mouse and keyboard version.
Both hands now can be any of four control modes. Press button 1 (A or X on an oculus touch) to switch modes. When you switch modes you will drop all held items. 
  Fly Mode: Text will appear directly above your hand
    Trigger - fly in the direction the controller is facing. Pressure changes speed
    Thumbstick up/down - change speed of flight
    thumbstick click and left/right - rotate camera in 45 degree incriments
    grip trigger - grab object.
  Teleport Mode:
    Trigger Pressed - starts teleportation. hold down and point where you would like to go
    Trigger Released - teleport to selected location
    Thumbstick - rotates the view on teleport landing (doesn't seem to work as intended)
    grip trigger - grab object
  Grab Mode:
    Grip trigger -  grab object
    Coming soon: thumbstick controls rotation of object and distance from hand
  Snapshot Mode: Your hand will turn into a camera viewport. 
    Trigger - take snapshot
    Thumb left/right - zoom in and out

Snapshots are saved to the {root}/Unreal/Snapshots where root is which drive you have the project downloaded to as HDR files. Photoshop will open them. There may or may not be a black line that appears on your snapshot, it is a known engine bug that will hopefully be fixed soon.

Roadmap:
  Add a laser pointer mode 

  make the camera snapshot tool vibrate on a capture
  ~~Create a visual tutorial level~~
  
  ~~Clean up the code and transition to using engine inputs instead of calling events directly in blueprint~~
  ~~16:9 format snapshots with the camera lens.~~ Add lens length and metadata to screencapture with a blackbar border
  
  ~~Change from preset hand controls to modes of control, press button 1 to open a control rotational picker, select new mode
      Modes to implement
        Flyaround motion
        teleport motion (may stay combined with flyaround)
        grab hand/place objects from "inventory" - spawn objects into the world like set dressing, traffic cones
        snapshot camera~~
        
        
      Modes to be considered
        various forms of cameras to create video imagry
        VR editor functionality such as scale, rotate, etc. 
        Open to suggestions
    Clean teleport function and make the rotation work
  teleport function and grab function are pulled from the unreal sample and need to be cleaned up
  camera should have the option to leave an image of the snapshot behind during runtime that could be copied to the game afterward
  Read the rest of my handwritten notes and upload them here.
  Create a mouse and keyboard version that autodetects the headset being off
  
