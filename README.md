export default function RimjimPortfolio() {
  const blogs = [
    {
      title: "Virtual Reality Hazard Hunt and Hazard Recognition for Effective Safety Training",
      link: "https://blog.infivr.com/virtual-reality-hazard-hunt-and-hazard-recognition-for-effective-safety-training/"
    },
    {
      title: "IOGP Line of Fire Immersive and AI-Powered Safety Trainings",
      link: "https://blog.infivr.com/infivrs-iogp-line-of-fire-immersive-and-ai-powered-safety-trainings/"
    },
    {
      title: "Bajaj Auto Reduces 65% Incidents and Safety Violations Using INFIVR AI 3D Fire Safety Trainings",
      link: "https://blog.infivr.com/bajaj-auto-reduces-65-incidents-and-safety-violations-using-infivr-ai-3d-fire-safety-trainings/"
    }
  ];

  return (
    <div className="min-h-screen bg-white text-gray-900 font-sans">
      {/* Hero Section */}
      <section className="px-6 md:px-20 py-20 bg-gradient-to-br from-gray-100 to-gray-200">
        <div className="max-w-6xl mx-auto grid md:grid-cols-2 gap-10 items-center">
          <div>
            <p className="uppercase tracking-[0.3em] text-sm text-gray-500 mb-4">
              Content Writer • Blog Writer • Marketing Enthusiast
            </p>
            <h1 className="text-5xl md:text-6xl font-bold leading-tight mb-6">
              Hi, I’m Rimjim Kamal.
            </h1>
            <p className="text-lg text-gray-700 leading-relaxed mb-8">
              I create engaging blog content, LinkedIn posts, and brand-focused writing that simplifies ideas and connects with people. From immersive tech blogs to marketing content, I enjoy turning information into stories that are easy to read and impactful.
            </p>

            <div className="flex flex-wrap gap-4">
              <a
                href="#work"
                className="px-6 py-3 rounded-2xl bg-black text-white hover:scale-105 transition"
              >
                View My Work
              </a>

              <a
                href="mailto:yourmail@example.com"
                className="px-6 py-3 rounded-2xl border border-gray-400 hover:bg-gray-100 transition"
              >
                Let’s Connect
              </a>
            </div>
          </div>

          <div className="bg-white rounded-3xl shadow-xl p-8 border border-gray-200">
            <h2 className="text-2xl font-semibold mb-4">About Me</h2>
            <p className="text-gray-700 leading-relaxed mb-4">
              I have experience in blog writing, LinkedIn content creation, and research-based writing. My work mainly focuses on technology, safety training, immersive learning, and marketing communication.
            </p>

            <div className="grid grid-cols-2 gap-4 mt-6">
              <div className="p-4 rounded-2xl bg-gray-100">
                <h3 className="font-semibold text-lg">Blogs Written</h3>
                <p className="text-gray-600">Industry & Tech Content</p>
              </div>

              <div className="p-4 rounded-2xl bg-gray-100">
                <h3 className="font-semibold text-lg">Content Focus</h3>
                <p className="text-gray-600">LinkedIn & Brand Writing</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Work Section */}
      <section id="work" className="px-6 md:px-20 py-20">
        <div className="max-w-6xl mx-auto">
          <div className="mb-12">
            <h2 className="text-4xl font-bold mb-4">Featured Writing</h2>
            <p className="text-gray-600 text-lg">
              A few blogs and content pieces I’ve worked on.
            </p>
          </div>

          <div className="grid md:grid-cols-3 gap-8">
            {blogs.map((blog, index) => (
              <div
                key={index}
                className="bg-white border border-gray-200 rounded-3xl p-6 shadow-sm hover:shadow-xl transition"
              >
                <div className="text-sm text-gray-500 mb-3">Blog Writing</div>
                <h3 className="text-xl font-semibold leading-snug mb-4">
                  {blog.title}
                </h3>

                <a
                  href={blog.link}
                  target="_blank"
                  rel="noopener noreferrer"
                  className="inline-flex items-center gap-2 text-black font-medium hover:underline"
                >
                  Read Article →
                </a>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* LinkedIn Section */}
      <section className="px-6 md:px-20 py-20 bg-gray-50">
        <div className="max-w-5xl mx-auto text-center">
          <h2 className="text-4xl font-bold mb-6">Social Content</h2>
          <p className="text-gray-700 text-lg leading-relaxed max-w-3xl mx-auto mb-10">
            Along with blog writing, I also create LinkedIn content focused on professional storytelling, brand communication, and audience engagement.
          </p>

          <a
            href="https://www.linkedin.com/feed/update/urn:li:activity:7439960956169863168"
            target="_blank"
            rel="noopener noreferrer"
            className="inline-block px-8 py-4 bg-black text-white rounded-2xl hover:scale-105 transition"
          >
            View LinkedIn Post
          </a>
        </div>
      </section>

      {/* CTA Section */}
      <section className="px-6 md:px-20 py-24">
        <div className="max-w-5xl mx-auto bg-black text-white rounded-[2rem] p-12 text-center shadow-2xl">
          <h2 className="text-4xl font-bold mb-6">
            Interested in working together?
          </h2>

          <p className="text-lg text-gray-300 leading-relaxed max-w-2xl mx-auto mb-8">
            If you’d like to discuss content writing, blog projects, internships, or job opportunities, feel free to connect with me.
          </p>

          <a
            href="mailto:yourmail@example.com"
            className="inline-block bg-white text-black px-8 py-4 rounded-2xl font-semibold hover:scale-105 transition"
          >
            Let’s Discuss Opportunities
          </a>
        </div>
      </section>

      {/* Footer */}
      <footer className="py-10 text-center text-gray-500 border-t border-gray-200">
        <p>© 2026 Rimjim Kamal • Portfolio Landing Page</p>
      </footer>
    </div>
  );
}
