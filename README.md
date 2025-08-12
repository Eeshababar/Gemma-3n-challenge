# 👁️ Intelligent Navigation Assistant for the Visually Impaired  


## 📌 Vision & Mission  
Empowering visually impaired individuals through a **free, charitable, intelligent navigation assistant**
Leveraging **offline multimodal AI** as "intelligent eyes," the system enhances **safety and autonomy** by delivering **real-time descriptive audio feedback** about environmental obstacles—enabling safe and confident navigation.  

Born at **Google – The Gemma 3n Impact Challenge**, we are committed to the **long-term non-profit development** of this technology.  

---

## 🚨 Problem Statement  
Navigating public and private spaces is challenging for people with visual impairments.  
Unexpected obstacles—such as benches, signs, discarded items, or temporary barriers—pose significant safety risks.  

While traditional aids like canes and guide dogs are invaluable, they **may not detect**:  
- Obstacles at **head height**  
- The **nature** of the obstacle  
- The **safest path** around it  

---

## 💡 Solution Overview  
Our solution combines a **smartphone camera feed** with a **two-tier AI architecture** to deliver real-time guidance:  

1. **Constant Scanning** – Google’s **MediaPipe** continuously scans for objects.  
2. **Intelligent Analysis** – When a significant object is detected, the **Gemma 3n multimodal model** is triggered.  
3. **Actionable Advice** – Gemma analyzes the scene, identifies hazards, and suggests safe navigation paths.  
4. **Audio Feedback** – Natural language descriptions are converted to **speech** for the user.  

**Example Output:**  
> "There is a bench directly in your path; it is safest to step to your right."

---

## ✨ Key Features  
- **Real-time Obstacle Detection** – Constant monitoring via smartphone camera.  
- **Intelligent Scene Analysis** – Context-aware hazard detection.  
- **Natural Language Audio Alerts** – Clear and concise voice feedback.  
- **Two-Tiered Architecture** – Efficient use of battery and compute.  
- **Accessibility-First Design** – Works with **TalkBack**, **haptic feedback**, and **high-contrast mode**.  

---

## 🛠 Technical Architecture  

```mermaid
flowchart LR
    A[Image Capture - CameraX] --> B[MediaPipe - Tier 1 Scanner]
    B -->|Significant Object Detected| C[Gemma 3n - Tier 2 Brain]
    C --> D[Hazard Description & Navigation Advice]
    D --> E[Text-to-Speech Output]
