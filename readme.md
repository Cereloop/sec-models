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


{
    "instruction": "Break down how to find the smallest measurable mass using LCM",
    "input": "4. Find the smallest mass that can be measured out in equal amounts of $10 \\mathrm{~g}$, $14 \\mathrm{~g}$, and $22 \\mathrm{~g}$.",
    "output": "**Step 1:** Factor each mass\n- $10 = 2 \\times 5$\n- $14 = 2 \\times 7$\n- $22 = 2 \\times 11$\n\n**Step 2:** Identify LCM\nMultiply the highest powers of all prime factors: $2^1 \\times 5^1 \\times 7^1 \\times 11^1 = 770$\n\n\boxed{770 \\text{ g}}\n\n⚠️ Common error: Confusing LCM with GCD (which gives the greatest common divisor instead of the smallest multiple)"
}

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

