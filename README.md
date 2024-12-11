                                   Blood Group Identification System


Overview:
      The Blood Group Identification System is a web-based application designed to identify blood groups by analyzing images of blood cells. It leverages Django for the backend and OpenCV for image processing to automate and simplify the traditionally manual process of blood typing. This system ensures quick, reliable, and accurate identification of both the ABO blood group and Rh factor.

Features:
      Automated Blood Typing: Identifies the ABO group and Rh factor from uploaded blood cell images.
      User Management:
      Registration and secure login.
      Personalized profile page to display results.
      Image Processing:
      Preprocessing images using techniques like grayscale conversion, thresholding, and morphological operations for accurate analysis.
      Dashboard Navigation: User-friendly interface for seamless access to the application features.
      Secure Data Storage: Stores user credentials and results securely in a structured database.

Tech Stack:
      Frontend:
            HTML
            CSS
      Backend:
            Django
      Image Processing:
            OpenCV
            Base64
      Database:
            SQLite

Installation:

Prerequisites:
       Ensure you have the following installed:
            Python (version 3.8 or higher)
            pip (Python package installer)
            Virtual environment (optional but recommended)
      Steps:
     1.  Clone this repository:
            git clone https://github.com/sumathi1205/Infosys-project.git
            cd blood-group-identification

     2.  Set up a virtual environment (optional but recommended):
            python -m venv venv
            source venv/bin/activate  # On Windows, use venv\Scripts\activate

     3.  Install the required packages:
            pip install -r requirements.txt
            
     4. Run migrations to set up the database:
            python manage.py migrate

     5. Start the Django development server:
            python manage.py runserver

     6. Access the application in your browser at http://127.0.0.1:8000.



How It Works:

    1. Registration & Login:
           New users register by entering basic details.
           Existing users log in securely to access their accounts.

    2. Image Upload:
          Users upload images of blood cells for analysis.
          
    3. Image Processing:
          The system preprocesses the uploaded image using OpenCV techniques:
          Converts the image to grayscale.
          Applies Gaussian blur to reduce noise.
          Thresholding highlights relevant features.
          Morphological operations refine contours for accurate analysis.
          
    4. Result Display:
          The system identifies the ABO group and Rh factor.
          Results, along with the processed image, are displayed on the user’s profile page.


Routes:


                    Route	                                Description
                    
                    /home	                                Main page introducing the system.
                    /about	                              Information about the project.
                    /contact	                            Contact details for support.
                    /service	                            Access to the blood group analyzer.
                    /login	                              User login page.
                    /register	                            User registration page.



![image](https://github.com/user-attachments/assets/b22a0f25-2d06-4337-9576-187226fc56ff)




Advantages:
      Error-Free: Automated process reduces human errors.
      Time-Saving: Processes results within seconds, critical during emergencies.
      User-Friendly Interface: Simplifies usage for medical professionals and individuals.
      Reliable Results: Leverages advanced algorithms for high accuracy.

outputs:

![image](https://github.com/user-attachments/assets/6d253982-bc97-4bcc-af34-2c077f8ff3ca)

![image](https://github.com/user-attachments/assets/4fd5ca0d-5e6a-4c93-89d3-c9a36ec8481c)

![image](https://github.com/user-attachments/assets/ab386a5c-d0d8-48be-ac99-ab2176d3f5a9)

![image](https://github.com/user-attachments/assets/589edaf4-0b65-443e-94fc-cff61bdacdd7)




      
Contributors:
     * Konatham Sumathi
     * Yuvashri Devi
     * Rajdeep Mondal

Future Scope:
      Integrate advanced AI/ML models for improved accuracy and speed.
      Expand support for additional blood tests or health parameters.
      Develop a mobile application for easier access.
