# Parking-Aid-with-Machine-Learning
This project is done in my final year of Undergraduate Studies (Bachelor of Technology in Computer Science and Engineering).

This Project deals with the problems of parking vehicles in humongous campuses with multiple parking spaces with no parking Allocation System.

**ABSTRACT** : Many Organizations have huge number of Employees or students. Most of those people travel by their vehicles. Because of this flood of vehicles, there rises the problem of parking them. These organizations have the land power to accommodate those many vehicles but do not have any reliable parking system.

The main objective of this project is to handle this situation of parking problems. We developed a system that can take care of parking problems by using a dynamic allocation policy. We recognize the vehicles as they come in through the entry gate, and the license number of that vehicle is extracted for logging. The images from the parking spaces are analyzed for free spaces and the incoming vehicle will be allocated an appropriate slot.

This License plate recognition is achieved in a step-by-step manner. First, an image from the entry gate is extracted, and then it is converted into a grayscale for ease of identification. Then later this grayscale is converted into a binary image for giving input to the KNN model. This KNN model is used to identify the total possible characters in the scene. By using these possible characters, the possible plates are identified. From these possible plates, the number plate of the vehicle is identified.

The image of the extracted number plate is given to the Tesseract OCR engine. This Tesseract OCR engine gives text as output when an image containing text is given as input. Our system can detect as many license plates in the image as possible.

In parallel to the above execution of the project, the images of all the parking spaces available are taken and are analyzed using a combination of imageai and the YOLOv3-Tiny pre-trained model. These models are used for object detection in parking slots. The total number of empty slots is plucked out and the incoming vehicle is allocated an appropriate slot. The program finally displays the output as the number plate of the vehicle followed by the parking slot number. If all the parking slots are full, it will display “Parking Full”.


P.S: The Images used in this project are tailor made for our institute
