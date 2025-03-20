# Cereloop - Open Source AI models for Nigerian Secondary School Education

Welcome to the Cereloop project! We are building lightweight, open-source AI instruct models tailored to the Nigerian secondary school curriculum. Our mission is to provide accessible, high-quality educational resources for students, particularly those with limited access to quality teachers and educational materials.

## Project Goal

To create AI models that can run on consumer devices, even offline, to:

- **Help Nigerian students prepare for WAEC, JAMB, NECO, and other national exams.**
- **Assist teachers in creating engaging and relatable teaching materials specific to the Nigerian context.**

## Subjects Covered

We are initially focusing on the following core subjects:

- Mathematics
- Chemistry
- Physics
- Biology
- (And potentially more in the future!)

## Current Status: Data Collection & Fine-Tuning

We are currently in the **data collection and fine-tuning phase**. We are collecting data in a specific format optimized for training instruction-following models.

### Data Format: Instruction Fine-Tuning

We are fine-tuning an instruct model, and the data is structured in JSON format with three key fields:

- `instruction`: This field contains a concise, action-oriented instruction for the model. Examples include "Solve this problem", "Explain the concept of...", "Break down how to...".
- `input`: This field provides the context or the specific problem the model should act upon. This could be a question from a past paper, a formula, a scenario, or any relevant information.
- `output`: This field contains the expected response from the model, which could be a step-by-step solution, an explanation, a summary, or any other appropriate output.

**Example:**


```json
{
    "instruction": "Explain place value using a Nigerian context example.",
    "input": "Place value is an important concept that is often misunderstood and sometimes misplaced. The decimal system depends on place value. This means, the value of a digit varies depending on its position. For instance in 345, the number '4' stands for forty or 4 tens whilst in 453 the value of the number '4' is four hundred. In 534 , the value of '4' is simply four since it is in the unit position. In 4350 , the value of 4 is four thousand since it is in thousands position. The numeral 82537 has 5 digits. This is read as 'eighty two thousand, five hundred and thirty seven. These five digits represent number of ones, a number tens, the number of hundreds, a number thousands and a number ten thousands. Table 1.1 shows the place value and the value of the digits in the numeral 82537.",
    "output": "Imagine you are sharing money with your friends. If you have ₦345, the 3 represents 300 Naira, the 4 represents 40 Naira, and the 5 represents 5 Naira. The *position* of the digit tells you how much it's worth! That's place value. So, the '4' in ₦345 is different from the '4' in ₦453, where it stands for 400 Naira. The '4' in ₦534 means only 4 Naira.\n\nIf you had ₦4350, the '4' means 4000 Naira. So, the same digit '4' can have different values depending on where it is in the number. Always remember to consider where the number is placed."
  },
```

## Contributing
We welcome contributions of all kinds!  Whether you're a data scientist, teacher, student, or just someone who cares about education in Nigeria, we encourage you to get involved.


## License

This project is licensed under the [Specify License, e.g., Apache 2.0 or MIT License]. See the `LICENSE` file for more details.

## Contact

For any questions or inquiries, please contact the Cereloop team at info@cereloop.com.

## Roadmap (Future Plans)

*   **Develop data processing pipelines to clean and annotate the collected data.**
*   **Train lightweight AI models for each subject, focusing on question answering and explanation generation.**
*   **Create a user-friendly interface for students and teachers to access the models.**
*   **Deploy the models on accessible platforms, including mobile devices and offline environments.**
*   **Partner with schools in Nigeria to pilot and evaluate the models.**

We believe that this project has the potential to make a significant impact on education in Nigeria. We are excited to have you join us on this journey!

