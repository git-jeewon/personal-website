<!-- Homepage with centered hero section -->
<svelte:head>
  <title>William Park - Full Stack Developer</title>
  <meta name="description" content="Personal website of William Park, a passionate full stack developer creating innovative web solutions." />
</svelte:head>

<!-- Hero Section -->
<section class="flex items-center justify-center min-h-[calc(100vh-4rem)] px-4 sm:px-6 lg:px-8">
  <div class="text-center max-w-3xl mx-auto">
    <!-- Name -->
    <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold text-gray-900 mb-6">
      <span class="block">Hello, I'm</span>
      <span class="block text-blue-600">William Park</span>
    </h1>
    
    <!-- Title -->
    <h2 class="text-xl sm:text-2xl md:text-3xl font-medium text-gray-700 mb-8">
      Full Stack Developer & Creative Problem Solver
    </h2>
    
    <!-- Tagline -->
    <p class="text-lg sm:text-xl text-gray-600 mb-12 leading-relaxed">
      I build modern, scalable web applications with clean code and thoughtful design. 
      Passionate about creating digital experiences that make a difference.
    </p>
    
    <!-- Call to Action Buttons -->
    <div class="flex flex-col sm:flex-row gap-4 justify-center">
      <a 
        href="/projects" 
        class="btn btn-primary text-lg px-8 py-3 inline-flex items-center justify-center"
      >
        View My Projects
        <svg class="ml-2 w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3" />
        </svg>
      </a>
      
      <a 
        href="wpark.jwon@gmail.com" 
        class="btn btn-secondary text-lg px-8 py-3 inline-flex items-center justify-center"
      >
        Get In Touch
        <svg class="ml-2 w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
        </svg>
      </a>
    </div>
  </div>
</section>

<!-- Brief Introduction Section -->
<section class="py-16 bg-white">
  <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="text-center mb-16">
      <h3 class="text-3xl font-bold text-gray-900 mb-6">About Me</h3>
      <div class="max-w-2xl mx-auto">
        <p class="text-lg text-gray-600 leading-relaxed mb-6">
          I'm a passionate developer who loves turning ideas into reality through code. 
          With expertise in modern web technologies, I focus on creating efficient, 
          scalable solutions that deliver exceptional user experiences.
        </p>
        <p class="text-lg text-gray-600 leading-relaxed">
          When I'm not coding, you can find me exploring new technologies, listening to music, 
          or enjoying the great outdoors.
        </p>
      </div>
    </div>
    
    <!-- Tech Stack Preview -->
    <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
      <div class="p-6 bg-gray-50 rounded-lg">
        <h4 class="font-semibold text-gray-900 mb-2">Frontend</h4>
        <p class="text-sm text-gray-600">React, Svelte, TypeScript</p>
      </div>
      <div class="p-6 bg-gray-50 rounded-lg">
        <h4 class="font-semibold text-gray-900 mb-2">Backend</h4>
        <p class="text-sm text-gray-600">Node.js, Python, APIs</p>
      </div>
      <div class="p-6 bg-gray-50 rounded-lg">
        <h4 class="font-semibold text-gray-900 mb-2">Database</h4>
        <p class="text-sm text-gray-600"></p>
      </div>
      <div class="p-6 bg-gray-50 rounded-lg">
        <h4 class="font-semibold text-gray-900 mb-2">Tools</h4>
        <p class="text-sm text-gray-600">Git, Docker, AWS</p>
      </div>
    </div>
  </div>
</section>
