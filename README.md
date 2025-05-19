# **Persist**  
### *The Universal Save System for Godot 4.x*  

**Effortlessly save and load game states** with a single line of code. Persist offers a **thread-safe, binary-encrypted** solution designed for production-ready games.  

```gdscript
# Save your game with one call
Persist.save(1)  

# Load it back just as easily  
Persist.load(1)
```

---

## **Features**  
✅ **One-line API** – Simple `save(slot)`/`load(slot)` interface  
✅ **Binary + Encryption** – Fast, compact, and secure saves  
✅ **Threaded Operations** – No more frame drops during saves  
✅ **Scene Persistence** – Automatically tracks scene changes  
✅ **Version Control** – Handles savefile migrations gracefully  
✅ **Modular Design** – Add `Saveable` to any node with 2 lines of code  

---

## **Why Persist?**  
- 🚀 **Competes with Unity/Unreal save systems** – All the features you need, built for Godot.  
- 🔒 **Security-first** – AES-256 encryption and checksum validation.  
- 📦 **Lightweight** – No dependencies, just pure GDScript performance.  

---

## **Quick Start**  
1. Add `persist.gd` as an autoload (`Persist`)  
2. Inherit from `Saveable` in nodes you want to persist:  
   ```gdscript
   extends CharacterBody2D
   class_name Player
   inherits Saveable  # <-- That's it!
   ```  
3. Implement `save_data()` and `load_data()` (see [examples](link-to-examples)).  

---

## **Roadmap**  
- [ ] Cloud save integration (Steam/Google Play)  
- [ ] Savefile screenshot thumbnails  
- [ ] Delta save optimizations  

---

**Perfect for**: RPGs, Roguelikes, Survival Games, and any project needing reliable state persistence.  

📜 **License**: MIT (free for commercial use)  

---

### **Why Developers Love It**  
> *"Persist replaced my messy JSON saves with a professional system in minutes. The threaded saves are a game-changer!"*  
> – *[User Testimonial]*  

---

