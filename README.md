## Inspiration
Every year, millions of tons of recyclables are incorrectly sorted and end up in landfills, driving up costs and causing significant environmental damage. This inefficiency affects educational institutions, commercial spaces, and waste management systems, which face high contamination fees and rising operational expenses. Despite ongoing educational efforts, schools and businesses continue to struggle with proper waste disposal and often fall short of their sustainability goals. We were inspired to create Sortify to address this gap by bringing clarity and accountability to everyday waste sorting. By integrating computer vision and AI into a low-cost, attachable device for trash cans, Sortify removes the guesswork from disposal decisions—making it easier for users to sort waste correctly in real time. Our primary focus is the educational sector, where current initiatives have proven insufficient, and where we see the greatest opportunity to make a lasting impact.

## What it does
Sortify is a smart, affordable device that attaches to any trash can and uses an AI-powered camera system to detect the type of waste being thrown away, such as food waste, recyclables, compost, and food containers, and provides real-time feedback to guide proper disposal. Through auditory alerts (e.g., buzzers), the system instantly informs the user if they’ve thrown something in the wrong bin. It is lightweight, low-cost ($28), cloud-connected, and designed to scale across schools, businesses, and waste management facilities​. It also collects data about what trash is being thrown away to ensure that this data can be passed onto janitors and anything dangerous can be sorted before being thrown out. The data can also be used to gamify the process between different educational institutions.

## How we built it
We built our MVP using:
- An ESP32-CAM for image capture and Wi-Fi connectivity
- A cloud-based image classification model powered by YOLOv8
- PIR sensors that activate the microcontroller only when necessary.
- A TP4056 charging module for reusability without constant power
- Buzzers to give immediate feedback when incorrect sorting occurs
We focused on keeping costs low to ensure scalability, with the whole system costing less than $30 while maintaining accuracy and performance. The model is trained on a limited number of high-frequency waste items to improve real-time classification speed and efficiency. Our beachhead market would be schools in Davis, California to help spread better educational experiences. 

## Challenges we ran into
- Balancing performance and cost: Keeping the model lightweight enough to run affordably while still providing reliable classifications was a key hurdle.
- Data collection & labeling: Obtaining and organizing images of various waste types in diverse contexts proved time-consuming.
- User behavior & edge cases: People throw away waste in unexpected ways: partially hidden items, dirty recyclables, overlapping objects, etc., which can confuse even well-trained models.
- Power supply: Designing a wireless, rechargeable system without requiring constant power while maintaining uptime was another challenge.

## Accomplishments that we're proud of
- Built a working prototype for under $30, well below the cost of existing smart bin solutions.
- Initiated pilot testing at two elementary schools and received positive early feedback.
- Developed a modular design that allows for easy retrofitting on existing waste bins.
- Created a clear business model with potential subsidies from waste management companies​

## What we learned
- Simplicity scales: Focusing on minimal components and a clean user interface can make adoption more practical in schools and commercial spaces.
- Education is key: Even with tech solutions, user understanding of waste categories plays a big role in success.
- Debugging: We learned how to use Tensorflow models and how to train a model using images of different food and compost items. 
## What's next for Sortify
- We want to pilot this program at elementary schools around Davis. We are going to outreach to UC Davis's Recycling facility and elementary schools to set up a program and prototype our product. We are also going to file for IP protection and applying to receive funding. 
