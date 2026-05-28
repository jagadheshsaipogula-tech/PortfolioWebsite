# PortfolioWebsite
export default function PortfolioWebsite() {
  const projects = [
    {
      title: "AI-Based Human Emotion Detection",
      description:
        "Developed a machine learning model capable of detecting and classifying human emotions from facial expressions using computer vision and deep learning algorithms for real-time emotion recognition.",
      tech: "React.js, Node.js, Machine Learning, Computer Vision"
    }
  ];

  return (
    <div className="min-h-screen bg-gray-100 text-gray-900">
      {/* Navbar */}
      <nav className="bg-black text-white p-4 flex justify-between items-center sticky top-0 shadow-lg">
        <h1 className="text-2xl font-bold">Jagadheshsai Pogula</h1>
        <div className="space-x-6">
          <a href="#about" className="hover:text-gray-300">About</a>
          <a href="#skills" className="hover:text-gray-300">Skills</a>
          <a href="#projects" className="hover:text-gray-300">Projects</a>
          <a href="#contact" className="hover:text-gray-300">Contact</a>
        </div>
      </nav>

      {/* Hero Section */}
      <section className="h-screen flex flex-col justify-center items-center text-center px-6 bg-gradient-to-r from-black to-gray-800 text-white">
        <h2 className="text-5xl font-bold mb-4">Hi, I'm Jagadheshsai Pogula</h2>
        <p className="text-xl max-w-2xl">
          Full-Stack Developer passionate about building responsive, modern, and AI-powered web applications.
        </p>
        <button className="mt-8 px-6 py-3 bg-white text-black rounded-2xl font-semibold hover:bg-gray-300 transition">
          Download Resume
        </button>
      </section>

      {/* About Section */}
      <section id="about" className="py-20 px-8 max-w-5xl mx-auto">
        <h2 className="text-4xl font-bold mb-8 text-center">About Me</h2>
        <div className="bg-white p-8 rounded-3xl shadow-lg">
          <p className="text-lg leading-8">
            I am currently pursuing B-Tech in Information Technology at Dhanekula Institute of Engineering and Technology. I am passionate about full-stack development and skilled in CSS, Node.js, React.js, and modern web technologies. I enjoy building innovative projects and solving real-world problems using technology and AI.
          </p>
        </div>
      </section>

      {/* Skills Section */}
      <section id="skills" className="py-20 bg-gray-200 px-8">
        <h2 className="text-4xl font-bold mb-10 text-center">Skills</h2>

        <div className="grid grid-cols-2 md:grid-cols-4 gap-6 max-w-5xl mx-auto">
          {[
            "Full-Stack Development",
            "CSS",
            "JavaScript",
            "React.js",
            "Node.js",
            "Express.js",
            "MongoDB",
            "GitHub"
          ].map((skill) => (
            <div
              key={skill}
              className="bg-white p-6 rounded-2xl shadow-md text-center font-semibold hover:scale-105 transition"
            >
              {skill}
            </div>
          ))}
        </div>
      </section>

      {/* Projects Section */}
      <section id="projects" className="py-20 px-8 max-w-6xl mx-auto">
        <h2 className="text-4xl font-bold mb-10 text-center">Projects</h2>

        <div className="grid md:grid-cols-3 gap-8">
          {projects.map((project, index) => (
            <div
              key={index}
              className="bg-white rounded-3xl shadow-lg p-6 hover:shadow-2xl transition"
            >
              <h3 className="text-2xl font-bold mb-4">{project.title}</h3>
              <p className="mb-4 text-gray-700">{project.description}</p>
              <p className="font-semibold">Tech Used:</p>
              <p>{project.tech}</p>
            </div>
          ))}
        </div>
      </section>

      {/* Contact Section */}
      <section id="contact" className="py-20 bg-black text-white px-8">
        <h2 className="text-4xl font-bold mb-10 text-center">Contact Me</h2>

        <div className="max-w-3xl mx-auto bg-gray-900 p-8 rounded-3xl shadow-lg">
          <div className="space-y-6">
            <input
              type="text"
              placeholder="Your Name"
              className="w-full p-4 rounded-xl text-black"
            />

            <input
              type="email"
              placeholder="Your Email"
              className="w-full p-4 rounded-xl text-black"
            />

            <textarea
              placeholder="Your Message"
              rows="5"
              className="w-full p-4 rounded-xl text-black"
            ></textarea>

            <button className="bg-white text-black px-6 py-3 rounded-2xl font-semibold hover:bg-gray-300 transition">
              Send Message
            </button>
          <div className="bg-gray-800 p-4 rounded-xl">
              <p><strong>Email:</strong> jagadheshsaipogula@gmail.com</p>
              <p><strong>Phone:</strong> 7386006198</p>
              <p><strong>GitHub:</strong> github.com/jagadheshsaipogula-tech</p>
              <p><strong>LinkedIn:</strong> www.linkedin.com/in/jagadhesh-sai-pogula-43a700374</p>
            </div>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-gray-950 text-white text-center py-6">
        <p>© 2026 Jagadheshsai Pogula. All Rights Reserved.</p>
      </footer>
    </div>
  );
}
