# Velocity - FPS Movement Shooter

A practice FPS game built in Unreal Engine 5 to explore advanced movement mechanics, weapon systems, and AI behavior.

Velocity is a portfolio project focused on implementing core FPS mechanics with emphasis on fluid movement and modular weapon design. Created as a learning exercise to deepen understanding of Unreal Engine's animation system, AI tools, and blueprint programming.

![akb64q](https://github.com/user-attachments/assets/d0aea891-fc29-46f8-87d6-87dc845f5200)

##  Features

### Movement System
- **Sprint** - Increased movement speed
- **Slide** - Momentum-based sliding with smooth animations
- Ground detection for movement validation

![akb61h](https://github.com/user-attachments/assets/0ee569b7-4626-4b01-8439-7b5066774660)

### Weapon System
- **Pistol** - Fast-firing pistol
- **Shotgun** - High-damage close-range weapon
- Reload animations with proper timing
- Fire animations with VFX
- Weapon-specific animation layers
- Ammo persistence between weapon switches
- Data-driven weapon configuration (Data Tables)

![akb677](https://github.com/user-attachments/assets/6a7485d5-a140-4b69-b6e0-d573c34a8451)



### AI System
- **Flying Dragon Enemy**
  - Ranged attacks (Fireball projectiles)
  - Player detection and pursuit


##  Technical Implementation

### Animation System
- **Animation Blueprint Layering** - Modular weapon animation system using Linked Anim Layers
- **Animation Layer Interface** - Allows dynamic swapping between weapon-specific animations
- **Montage System** - Fire and reload actions using Animation Montages
- **Procedural Aiming** - Transform (Modify) Bone for camera-follow aim

### Weapon Architecture
- **Base Weapon Class** (BP_WeaponBase) with child blueprints for each weapon type
- **Weapon Component** (AC_WeaponHandler) managing equip, fire, reload logic
- **Data Structure** (S_Weapons) storing weapon properties
- **Data Table** (DT_Weapons) for easy weapon configuration and balancing
- **Map-based ammo tracking** for persistence across weapon switches

##  What I Learned

- **Animation Blueprint Systems** - Creating modular animation layers that swap based on equipped weapon
- **Data-Driven Design** - Using structures and data tables for scalable weapon configuration
- **AI Programming** - Implementing Behavior Trees and Blackboards for enemy decision-making
- **Component Architecture** - Separating concerns with Actor Components (WeaponHandler)
- **State Management** - Handling weapon switching, ammo persistence, and reload states
- **Blueprint Best Practices** - Proper casting, variable management, and execution flow



##  Controls

- **WASD** - Movement
- **Shift** - Sprint
- **Ctrl** - Slide
- **Left Mouse** - Fire
- **R** - Reload
- **1** - Equip Pistol
- **2** - Equip Shotgun 


##  Built With

- **Unreal Engine 5.5**
- **Blueprints** 

##  Development Notes

This project was created as a learning exercise to understand:
- How modern FPS games structure their weapon systems
- The relationship between animation blueprints and gameplay code
- Proper blueprint architecture and organization

All systems are designed to be modular and extensible for future additions.

##  Contact


- LinkedIn: [(https://www.linkedin.com/in/alper-ikiz-587a201a3/)]
- Email: [ikiz19@itu.edu.tr]

---

**Note:** This is a learning project and not intended for commercial release.
