# Kietemo

```text
 __   ___   __     _______  ___________  _______  ___      ___     ______    
|/"| /  ") |" \   /"     "|("     _   ")/"     "||"  \    /"  |   /    " \   
(: |/   /  ||  | (: ______) )__/  \\__/(: ______) \   \  //   |  // ____  \  
|    __/   |:  |  \/    |      \\_ /    \/    |   /\\  \/.    | /  /    ) :) 
(// _  \   |.  |  // ___)_     |.  |    // ___)_ |: \.        |(: (____/ //  
|: | \  \  /\  |\(:      "|    \:  |   (:      "||.  \    /:  | \        /   
(__|  \__)(__\_|_)\_______)     \__|    \_______)|___|\__/|___|  \"_____/    
```

## About

**Kietemo** is an experimental Unreal Engine project heavily inspired by my love for FPS and survival games, the combat and progression systems of games such as *Sekiro*, Japanese samurai manga such as *Vagabond* and *The Blade of the Immortal*, and Japanese folklore surrounding Yokai.

The project began during COVID as a personal attempt to combine these influences into a large-scale survival horror game.

Kietemo was originally developed in **Unreal Engine 4** and later ported to **Unreal Engine 5**. Development was eventually abandoned as the scope of the project grew beyond what my hardware and available time could support.

The original project also became difficult to recover due to Unreal Engine's rapid version changes and my limited understanding of source control at the time. The original GitHub history is therefore relatively sparse, and the project no longer builds cleanly in its original state.

Rather than treating the project as lost, I am revisiting it as a **technical revival**: reconstructing the systems that made the original project interesting, modernizing the implementation, and documenting what I learned from the original development process.

## Combat

Combat was heavily inspired by **Sekiro** and other timing-focused melee games.

The goal was to make fighting dangerous rather than simply reducing combat to health-bar management.

The original implementation was primarily developed using **Unreal Engine Blueprints**, with experimentation around responsive melee interactions, enemy behavior, and player combat states.

The intention was for different enemy classes to require different approaches rather than allowing one universal combat strategy.

---

# Engineering Highlights

## Procedural Terrain Generation

One of the primary technical systems is procedural world generation.

**Perlin noise** is used to generate terrain and influence the distribution of environmental features.

The original implementation was written in **C++** and was intended to support the generation of large, potentially continuous territories.

The system was experimented with for:

* terrain height generation;
* environmental variation;
* structure placement;
* regional differences;
* and creating the illusion of a much larger world from procedural rules.

This was one of my earliest experiments with procedural generation and eventually became one of the reasons I became interested in the technical side of game development.

---

## Unreal Engine / C++

The project combines **C++ and Unreal Engine's gameplay framework** with Blueprint-based gameplay systems.

C++ was primarily used where lower-level control and procedural computation were useful, while Blueprints were used extensively for gameplay logic and rapid iteration.

This hybrid approach allowed me to experiment quickly while still learning how Unreal's native systems interacted with higher-level gameplay logic.

---

## Blueprint Combat Systems

The combat system was implemented primarily through Blueprints.

The original goal was to experiment with:

* attack states;
* enemy reactions;
* timing-based combat;
* player/enemy interactions;
* animation-driven gameplay;
* and combat behavior inspired by Sekiro.

Because the project was developed while I was still learning Unreal Engine, many of these systems are experimental rather than production-ready.

---

# Technical Revival

The current goal of this repository is **not simply to restore the original project exactly as it existed**.

The original project relied on an older Unreal Engine version and has accumulated compatibility issues over time.

The revival therefore focuses on:

* identifying which original systems can be recovered;
* reconstructing systems that can no longer be directly recovered;
* updating obsolete Unreal Engine implementations;
* improving project organization;
* documenting technical decisions;
* and rebuilding important systems using modern Unreal Engine practices.

The original implementation is preserved where practical so that the evolution of the project can be understood.

---

# What I Learned

Kietemo was one of my earliest attempts at building a large-scale game system.

It taught me several lessons that were difficult to appreciate while I was developing it:

* **Scope matters.** A game can become technically impossible to maintain long before the individual systems become difficult.
* **Source control matters.** Keeping a project in a working state is as important as writing the code itself.
* **Engine versions matter.** Large engine migrations can invalidate assumptions throughout an entire project.
* **Procedural generation requires careful design.** Generating a large world is considerably easier than generating one that is interesting.
* **Architecture matters.** Rapid prototyping can create significant technical debt when a project grows.
* **Documentation matters.** Years later, undocumented systems become significantly harder to understand and recover.

This revival is therefore also an opportunity to revisit some of my earliest engineering decisions and see how I would approach the same problems today.

---

# Status

**Project status: Revival / Experimental**

The original project is no longer fully functional in its original Unreal Engine environment.

The current work focuses on selectively recovering and modernizing the most interesting systems rather than attempting to restore the entire original game at once.

### Planned / Experimental Systems

* [ ] Modernize procedural terrain generation
* [ ] Rebuild Perlin noise implementation
* [ ] Reconstruct procedural structures
* [ ] Rebuild combat systems
* [ ] Revisit enemy AI
* [ ] Reconstruct spiritual starvation system
* [ ] Experiment with dynamic world regions
* [ ] Improve project architecture
* [ ] Document technical implementations
* [ ] Produce playable prototypes of recovered systems

---

# Keywords

**Unreal Engine · C++ · Blueprints · Procedural Generation · Perlin Noise · Game Development · Survival Horror · FPS · Samurai · Yokai · Japanese Folklore**

```
```
