# Normalizing-Flow-Models
# RealNVP Network on make_moons Dataset

**What is make_moons data?**

make_moons is a function from the Python library sklearn that generates a simple dataset shaped like two interlocking crescent moons. It's commonly used for testing machine learning algorithms because it creates a non-linear pattern in the data.

Here’s a breakdown:

Crescent Moons: The dataset consists of two sets of points that look like crescent moons or arches.

Classification Task: It’s often used for classification tasks, where the goal is to separate the two moon-shaped groups (or classes).

Noise: You can add some noise to make the dataset more challenging to separate perfectly.

In simple terms, make_moons creates two clusters of points that aren't in a straight line but have a curved shape, making it useful for testing how well algorithms handle more complex shapes in data.

**Goal of RealNVP:**

The RealNVP (Real-valued Non-Volume Preserving) model transforms complex data, like the two crescent moons from the make_moons dataset, into a simpler distribution, such as a Gaussian distribution. The Gaussian, or normal distribution, is a bell-shaped curve that represents a pattern where most of the data points are clustered around the center.

**Training Process:**

As the model trains, it tries to learn a transformation that takes the make_moons data and reshapes it into a Gaussian-like form. This transformation is learned by minimizing the loss.

**Loss Curve Explanation:**

In the graph, the loss starts high because at the beginning, the model is not good at transforming the data into a Gaussian distribution.
Over time, as the model learns, the loss decreases. This shows the model is getting better at reshaping the make_moons data into a simpler, more Gaussian-like form.
The curve flattens out after a while, meaning the model has learned the transformation well and further improvements are minimal.

**How It Relates to Gaussian Distribution:**

The lower the loss, the better the model is at transforming the original complex distribution (like the moon shapes) into a Gaussian distribution. So, while the graph shows loss over time, it indirectly represents how well the data is being transformed into a Gaussian distribution as the loss decreases.

**Conclusion**

In this assignment, we successfully built a RealNVP model that can transform a complex data distribution like make_moons into a simple Gaussian distribution. The model's performance, as shown in the loss curve, closely matches the results presented in the book.

The key takeaway is that normalizing flows like RealNVP can provide a powerful way to learn invertible mappings between distributions while maintaining tractable density estimation. This makes them suitable for a variety of generative modeling tasks.

In conclusion, the RealNVP network effectively learns to capture the complexity of the data distribution, transforming it into a simpler form. Our model’s convergence and performance are on par with the results provided in the book, demonstrating the success of the method.

**REFERENCES**

Alshedivat, M., & Salakhutdinov, R. (2021). Normalizing flows: RealNVP and extensions. In Generative deep learning: Tools and techniques for building generative models (2nd ed.). O’Reilly Media. Retrieved from https://github.com/davidADSP/Generative_Deep_Learning_2nd_Edition/blob/main/notebooks/06_normflow/01_realnvp/realnvp.ipynb









