<!-- Projects page with project cards -->
<script>
  // Hardcoded project data - easy to customize later
  const projects = [
  ];
</script>

<!-- Page head -->
<svelte:head>
  <title>Projects - Your Name</title>
  <meta name="description" content="Explore my portfolio of web development projects, from e-commerce platforms to APIs and more." />
</svelte:head>

<!-- Projects Header -->
<section class="bg-white py-16">
  <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="text-center mb-16">
      <h1 class="text-4xl sm:text-5xl font-bold text-gray-900 mb-6">
        My Projects
      </h1>
      <p class="text-xl text-gray-600 max-w-3xl mx-auto leading-relaxed">
        Here's a collection of projects I've worked on, showcasing different technologies 
        and approaches to solving real-world problems.
      </p>
    </div>
  </div>
</section>

<!-- Projects Grid -->
<section class="py-16 bg-gray-50">
  <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      {#each projects as project}
        <article class="bg-white rounded-xl shadow-lg overflow-hidden hover:shadow-xl transition-shadow duration-300">
          <!-- Project Image -->
          <div class="aspect-video bg-gradient-to-br from-blue-500 to-purple-600 flex items-center justify-center">
            <img 
              src={project.imageUrl} 
              alt={project.name}
              class="w-full h-full object-cover"
              loading="lazy"
            />
          </div>
          
          <!-- Project Content -->
          <div class="p-6">
            <!-- Project Title -->
            <h3 class="text-xl font-bold text-gray-900 mb-3">
              {project.name}
            </h3>
            
            <!-- Project Description -->
            <p class="text-gray-600 mb-4 leading-relaxed">
              {project.description}
            </p>
            
            <!-- Technologies -->
            <div class="mb-6">
              <h4 class="text-sm font-semibold text-gray-700 mb-2">Technologies:</h4>
              <div class="flex flex-wrap gap-2">
                {#each project.technologies as tech}
                  <span class="px-3 py-1 bg-blue-100 text-blue-800 text-xs font-medium rounded-full">
                    {tech}
                  </span>
                {/each}
              </div>
            </div>
            
            <!-- Project Links -->
            <div class="flex gap-3">
              {#if project.demoUrl}
                <a 
                  href={project.demoUrl}
                  target="_blank"
                  rel="noopener noreferrer"
                  class="btn btn-primary flex-1 text-center inline-flex items-center justify-center"
                >
                  <svg class="w-4 h-4 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14" />
                  </svg>
                  Live Demo
                </a>
              {/if}
              
              {#if project.githubUrl}
                <a 
                  href={project.githubUrl}
                  target="_blank"
                  rel="noopener noreferrer"
                  class="btn btn-secondary flex-1 text-center inline-flex items-center justify-center"
                >
                  <svg class="w-4 h-4 mr-2" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                  </svg>
                  GitHub
                </a>
              {/if}
            </div>
          </div>
        </article>
      {/each}
    </div>
  </div>
</section>

<!-- Call to Action -->
<section class="bg-white py-16">
  <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
    <h2 class="text-3xl font-bold text-gray-900 mb-6">
      Interested in Working Together?
    </h2>
    <p class="text-lg text-gray-600 mb-8 max-w-2xl mx-auto">
      I'm always open to discussing new opportunities and interesting projects. 
      Let's connect and see how we can create something amazing together.
    </p>
    <a 
      href="wpark.jwon@gmail.com"
      class="btn btn-primary text-lg px-8 py-3 inline-flex items-center justify-center"
    >
      Get In Touch
      <svg class="ml-2 w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
      </svg>
    </a>
  </div>
</section> 