# Flow Board – Background Configuration

## 🎯 Goal
Each Flow Board should have its own individually stored background configuration.  
The background is defined in the board settings (Classic mode) and is persistent across sessions.  

---

## 📌 Requirements
- Add a new field in the **Settings** tab of the Board Designer (Classic mode).  
- Field type: **Dropdown**, with predefined options:  
  - Standard  
  - Mountains  
  - Water  
  - Wood  
  - Forest  
  - Sky  
  - Winter  
  - Summer  
- Selection is saved **per board**.  
- The configured background is automatically applied when the board is opened in Flow mode.  
- The background applies to **all users** of a board.  
- Only users with the required permission can change the field.  

---

## 🚫 Non-Goals
- No per-user individual backgrounds.  
- No option for custom image uploads.  
- No changes to card/workflow behavior.  

---

## 📌 Assumptions
1. The Flow UI background logic cannot be reused directly in the configuration page, since the configuration uses a different technology (“Classic mode”). However, **standard dropdown components** from Classic mode can be used.  
2. **Role and permission logic** already exists in Classic mode for single fields. This must also be enforced in Flow mode to ensure the background cannot be changed by unauthorized users.  
3. Users without edit rights will see the configured background but cannot change it.  
