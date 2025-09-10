# The Aethereal Shop Kit  

Welcome! This guide will help you get started with **The Aethereal Shop Kit**.  
Follow the step-by-step instructions below to quickly build a world without starting completely from scratch.  

1. [Getting started](#1-getting-started)
2. [AD Panel](#2-the-ad-panel)
3. [Info Panel](#3-info-panel)
4. [Sliding Doors](#4-sliding-doors)

---
Watch the tutorial on YouTube

[![Watch the video](https://img.youtube.com/vi/zI97uj-i-D4/hqdefault.jpg)](https://www.youtube.com/embed/zI97uj-i-D4)

## 1 Getting Started  

### 1 Import the Kit  
1. Open **Horizon Worlds**  
2. Import the **Aethereal Shop Kit** into your project  

### 2. Place the Template  
1. Drag and drop the **template asset** into your space  
2. (Recommended) Enable **grid snapping** when using the move tool to align objects precisely  
<img width="1308" height="48" alt="image" src="https://github.com/user-attachments/assets/c7cfe90f-48aa-4435-afbe-0caa54866d80" />

---

## 1.1 Working with Kit Pieces  

1. Select the piece you want to use  
2. **Duplicate it** first  
3. Ungroup it from the main kit  
4. Remove it from its parent  
5. Reset its position by setting:  
   - **X: 0 | Y: 0 | Z: 0**  

Now you can duplicate and reuse that piece as many times as you need.  
Repeat this process for every object you want to extract from the kit.  

---

## 1.2 Building Structures  

1. Place **walls** and **arches** next to each other  
2. Rotate them to form **corners**  
3. Add **ceiling pieces** on top to complete the structure  

With just a few simple steps, you can assemble a wide variety of custom buildings.  

---

## 1.3 Preparing Sliding Doors  

1. Rotate and position the sliding doors where you want them  
2. Set **grid snapping** to **0.25** for accurate alignment  

That’s it — your sliding doors are ready to go!

# 2 The AD Panel
In this section we will see the Ad Panel functionalities

<img width="288" height="258" alt="image" src="https://github.com/user-attachments/assets/c045f6b5-557c-41db-a79f-9cf5b24956c0" />


## 2.1 Image props

To upload your custom images, you need to add textures to your project.

Go to Asset **Library > My Assets**.

Click **Add New > Texture > Choose files on your device**.

<img width="401" height="303" alt="image" src="https://github.com/user-attachments/assets/8de4bade-59a7-4e5f-9e7c-2a4daa02d4af" />

Now go to your Ad Panel and click on one of the image props.

<img width="290" height="169" alt="image" src="https://github.com/user-attachments/assets/7463c457-b887-4304-80db-118c7b84dc00" />

Select your uploaded image

<img width="346" height="221" alt="image" src="https://github.com/user-attachments/assets/8dcf9258-cae0-4c21-805d-84b9cb6dd5d7" />

We recommend uploading images that share the same aspect ratio.


## 2.2 Loop seconds prop

Editing this prop determines the image loop interval in seconds.

<img width="291" height="28" alt="image" src="https://github.com/user-attachments/assets/20154a1f-5843-4560-8080-60ecd44bc02c" />

## 2.3 Panel dimensions
The panel dimensions are defined by **panelWidth** and **panelHeight**. We strongly recommend setting the dimensions to match your uploaded images’ aspect ratio. (For example, if your images are 1920x1080, keep the aspect ratio at 16:9.)

<img width="291" height="59" alt="image" src="https://github.com/user-attachments/assets/0e1efb7a-9b0e-49ef-8982-d593b1fdc8ab" />

# 3 Info Panel

## 3.1 Change Info Panel Title, Description and Button text

To change info panel title and description edit the "title" and "description" sections of the script
<img width="293" height="114" alt="image" src="https://github.com/user-attachments/assets/1119be9e-4036-487f-8cc2-59cf3ef7ccfb" />

## 3.2 Info Panel Image
For the image you need to upload a Texture Asset first

Go to Asset **Library > My Assets**.

Click **Add New > Texture > Choose files on your device**.

<img width="401" height="303" alt="image" src="https://github.com/user-attachments/assets/8de4bade-59a7-4e5f-9e7c-2a4daa02d4af" />

Go to your info panel and click on the image prop, then select you image

<img width="293" height="117" alt="image" src="https://github.com/user-attachments/assets/b3e42cfb-9c4c-4875-a5df-0eb586ad6f2b" />

And you're done!

# 4 Sliding Doors

## 4.1 Upload Your Custom Door Assets  

To use your own doors, you first need to upload your 3D model.  

1. Open **Asset Library > My Assets**  
2. Click **Add New > 3D Model > Choose files on your device**  
3. Select and upload your door model  

<img width="348" height="363" alt="image" src="https://github.com/user-attachments/assets/7e70afe6-019f-4e40-9f44-ab35643de067" />

---

## 4.2 Replace Default Doors  

1. In the **Hierarchy**, delete **SlidingDoorRight**.  
2. Drag your uploaded door asset into the scene under the SlidingDoors object.  
3. Set its position to: **X: -2 | Y: 0 | Z: 0**  

<img width="292" height="104" alt="image" src="https://github.com/user-attachments/assets/296f50a1-b30e-4ca0-8e19-16fd8f217b93" />  

4. (Optional) Right-click the asset and select **Rename** to give it a custom name.  
5. Repeat the process for **SlidingDoorLeft**, setting its position to: **X: 2 | Y: 0 | Z: 0**.  

Next, open the **Trigger Object** in the Hierarchy and assign both sliding door objects in the script:  

<img width="317" height="166" alt="image" src="https://github.com/user-attachments/assets/41bf8378-81af-4fc5-aff2-adba3856a931" />

---

## 4.3 Configure Open Positions  

To set the open positions of the doors:  

1. Delete **slidingDoorRightOpen** from the Hierarchy.  
2. Duplicate **SlidingDoorRight**  
   - **Right-click > Duplicate Selection**  
3. Rename the duplicated object (e.g., `SlidingDoorRightOpen`).  
4. Move it to the desired open position.  
5. Disable its visibility in the panel:  

<img width="292" height="55" alt="image" src="https://github.com/user-attachments/assets/a0109436-a0ab-431d-bc0c-12fe05b00094" />  

6. Assign the duplicated object to the **Trigger Object’s script**:  

<img width="290" height="55" alt="image" src="https://github.com/user-attachments/assets/ad4f66c9-2768-4686-98f7-585c525ffb1a" />

Repeat the same steps for the **SlidingDoorLeft** if needed.  

---

## 4.4 Adjust Door Speed  

To change how fast the doors move, edit the **`moveDurationMs`** parameter inside the **Trigger Object script**:  

<img width="299" height="31" alt="image" src="https://github.com/user-attachments/assets/6d8fb217-cee8-4f30-87ac-72c07db7cbee" />  

Increase the value for slower movement, or decrease it for faster movement.  
