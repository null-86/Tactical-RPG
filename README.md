# Tactical-RPG
Summary: This is a tactical rpg game made in Unity (C#). Units move on a grid and deal damage to each other depending on their equipped weapons, items, individual stats, and terrain defense values. Weapons also have skills that activate on an event basis. If you're familiar with Fire Emblem, this is my attempt to make a game in that style. Dialogue and events can be triggered at any point during combat. Different enemies need different "AI" (Polymorphism). Combat is handled via Command Pattern.

Issues: Many issues have been resolved, but here are some of the biggest that I worked through.

1. Original design included some tightly coupled classes that took a great deal of work to decouple.
2. Data Persistence was tacked on late in development, but it should've been a consideration from the start.
3. UI was originally specific to each scene, but that didn't scale well. I later realized that I should re-use the UI components so that I only needed to edit a single object. 

Lessons learned: 
UX was better than my earlier projects, but I still need to work on it. I also learned firsthand the importance of Design Patterns, particularly the Factory and Command patterns as the entire combat system hinges on those. I also used a State Machine to control the combat phase. 
