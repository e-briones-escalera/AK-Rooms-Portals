# AK Rooms and Portals – Unity + Wwise

This is a case study focused on implementing **Audiokinetic (Wwise) Rooms & Portals** for spatial audio propagation inside an existing 3D game environment. It was developed as part of my final film school project, where my team and I were responsible for the entire audio pipeline and implementation.  

The goal of this implementation was to design a realistic and optimized spatial audio system where sounds dynamically travel through connected spaces, enhancing immersion and player awareness.

⚠️ **Disclaimer:** This project is part of my technical portfolio. Code, assets, and design are not licensed for reuse or distribution.  
> [Gameplay (Credits in the Description)](https://youtu.be/Sofi1LHqK9M?si=I2uuN4TZ0TNWN4rx)  

### Audio System Highlights
- Wwise Rooms & Portals used to simulate how audio propagates between enclosed areas, since the game had rooms from different sizes, I chose to use this system to make it more immersive for the player.  
- Optimized sound attenuation and reverb transitions as players move through different rooms.  
- Dynamic opening/closing portal logic synchronized with doors and level geometry.  
- Performance-aware design to reduce CPU overhead while maintaining spatial accuracy.  

### Integration Breakdown
- Fully modular setup in Unity. Wwise for room and portal management.  
- Automated room assignment for new level geometry to avoid manual, hard-coded setups.  
- Real-time debug visualizers in Wwise to confirm sound propagation paths.  
- Audio events integrated with gameplay triggers and environmental logic.  

### QA & Debugging Approach
- In-game visualization of active rooms and connected portals.  
- Edge-case testing for overlapping volumes, simultaneous portal triggers, and occluded paths.  
- Logged transitions and propagation changes to quickly identify misconfigurations.  

### Tech & Tools Used
- Unity
- Wwise (Audiokinetic)  
- Pro Tools 

## Credits
- Leaders of Implementation, Technical Sound Designers: Santiago Guerra & Estefania Briones
- Voice actress (La Coyota): Kendyl Twa
- AkRooms & Spatial Audio: Estefania Briones
- Audio Programmer: Santiago Guerra
- DX: Santiago Guerra
- Foley: Santiago Guerra
- Ambience: Estefania Briones
- Design & Implementation Sfx (vast majority): Santiago Guerra & Estefania Briones
- Sound Design Sfx and Wwise Motion: Raj Gill
- Music: Benjamin Ruiz
- Mentors: Alfonso Salinas, Andres Pineda, Matheus Vilano, Judy Kim
