# Creating a Knowledge Base

## **What is a Knowledge Base**

A knowledge base is a collection of files, links & external data sources an AI model can use to answer queries. This is built on state-of-the-art technologies like a vector store & RAG.

---

## **How to Setup a Knowledge Base?**

Follow these steps to configure a knowledge base. In this tutorial, we’ll create a knowledge base which has data about Airbnbs in it (the document will contain wifi details, emergency contacts etc) we’ll call it “Airbnb Database”, we’ll then test our AI bot can answer queries related to it. You can download the pdf we use in this demo [here](https://Messcat-media-store.s3.ap-east-1.amazonaws.com/8ce5f25e8b018ce5)

### **1. Access the AI ChatBot Setup**

1. Hover over the **“AI”** section in the left-hand sidebar, click on **“Knowledge Base”** and then click on **“+ Create”**.
    
    ![Screenshot 2025-04-14 at 5.30.26 PM.png](Creating%20a%20Knowledge%20Base/Screenshot_2025-04-14_at_5.30.26_PM.png)
    
2. Let’s name the Knowledge Base. For this demo, we’ll call it “Airbnb Info”
    
    ![Screenshot 2025-04-14 at 6.01.27 PM.png](Creating%20a%20Knowledge%20Base/Screenshot_2025-04-14_at_6.01.27_PM.png)
    

---

### **2. Add Training Data**

- **Option 1: Upload Files**
    - Upload **PDF, DOC, DOCX, TXT** documents that contain text data. Image data cannot be read by the AI
    - Click the “Upload a File” button and select files (1 or more)
        
        ![Screenshot 2025-04-14 at 6.03.57 PM.png](Creating%20a%20Knowledge%20Base/Screenshot_2025-04-14_at_6.03.57_PM.png)
        
    - It’ll save the changes in the knowledge base and upload the files
        
        ![Screenshot 2025-04-14 at 6.05.11 PM.png](Creating%20a%20Knowledge%20Base/Screenshot_2025-04-14_at_6.05.11_PM.png)
        
- **Option 2: Fetch from Website**
    - Coming Soon!
    
    <aside>
    ❗
    
    **Note**: Depending on the volume of data, the bot may take several minutes to fetch all the information.
    
    </aside>
    
- **Option 3: Connect Live Database**
    - Coming Soon!

---

### **3. Test the Knowledge Base**

![Screenshot 2025-04-14 at 6.06.12 PM.png](Creating%20a%20Knowledge%20Base/Screenshot_2025-04-14_at_6.06.12_PM.png)

Once you’ve added your files, you can change the **prompt** & **model** to test the knowledge base. You can test by sending files too.

- The model can be configured as:
    - **Gpt4oMini** — best for short context windows, fast responses & understanding textual queries.
    - **Gpt4o** — best for complex tasks, and If you expect your users to send images, and documents. Slower than the mini model
- The prompt is just as important as the knowledge you upload into the database. We’ll keep a simple one for now:
    
    > Act like a helpful AI assistant managing a multi location airbnb business, that will look through your files, and tools to assist in any queries users about the following:
    - wifi details and password
    - directions
    - toilet location
    - emergency dealings (including damage, physical threats etc.)
    
    If you do not know the airbnb the person is staying at, ask them. Do not send any data without knowing this information
    
    Greet the user, by their name if available, let them know you're an AI assistant and what things you can help them with. Do not tell the user about what files, or tools you have access to.
    > 

Now let’s test the knowledge base! Type in a message and see the results

![Screenshot 2025-04-14 at 6.20.23 PM.png](Creating%20a%20Knowledge%20Base/Screenshot_2025-04-14_at_6.20.23_PM.png)

### **4. Deploying the Knowledge Base to Users**