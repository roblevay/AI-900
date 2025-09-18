
---

## 🛠 Steg-för-steg: Aktivera Vision + Document i Azure AI Foundry

### 1. Skapa en **Azure AI Vision-resurs**

1. Logga in på [Azure Portal](https://portal.azure.com).
2. Klicka på **Create a resource** (”Skapa en resurs”).
3. Sök efter **Computer Vision**
4. Klicka på **Create**.
5. Fyll i:

   * **Subscription**: välj din (du har ”Betala per användning”).
   * **Resource group**: välj samma som för Foundry (t.ex. *airg3*).
   * **Region**: välj samma som Foundry (hos dig *westeurope*).
   * **Name**: t.ex. `robert-vision`.
6. Klicka **Review + Create** och sedan **Create**.

---

### 2. Koppla resursen till ditt Foundry-projekt

1. Gå till **Azure AI Foundry** → välj ditt projekt (*robert-westeur*).
2. Under **Project details** ser du ”Connect resources”.
3. Klicka där och lägg till din nya **Azure AI Vision**-resurs.

---

### 3. Använd Vision + Document

När resursen är kopplad kan du använda den på två sätt:

#### a) Via **Playgrounds** i AI Foundry

* Gå till **Playgrounds** i vänstermenyn.
* Där ska du nu se **Vision + Document**-funktioner (OCR, bildanalys, dokumenttolkning).

#### b) Via API

* Under **Endpoints and keys** i Foundry hittar du API-nyckeln och endpoint.
* Använd dessa för att anropa Vision API, t.ex. för OCR, dokumentanalys eller bildtolkning.
* Exempel på endpoint (din blir liknande):

  ```
  https://<ditt-namn>.cognitiveservices.azure.com/
  ```

---

### 4. Testa med OCR eller dokumenttolkning

* Ladda upp en bild eller PDF via Playground.
* Välj ”Extract text” eller ”Analyze document”.
* Du får då ut text och metadata direkt i Foundry.

---

👉 Efter detta har du alltså samma funktioner som den gamla *”AI Services → Vision + Document”*-knappen gav – men nu i det nya gränssnittet.

---


