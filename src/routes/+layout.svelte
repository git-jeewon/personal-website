<!-- Main layout for the personal website -->
<script>
  import '../app.css';
  import { page } from '$app/stores';
  
  // Navigation items
  const navItems = [
    { href: '/', label: 'Home' },
    { href: '/projects', label: 'Projects' }
  ];
</script>

<!-- Navigation -->
<nav class="bg-white border-b border-gray-200 sticky top-0 z-50">
  <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between h-16">
      <!-- Logo/Brand -->
      <div class="flex items-center">
        <a href="/" class="text-xl font-bold text-gray-900 hover:text-blue-600 transition-colors">
          William Park
        </a>
      </div>
      
      <!-- Navigation Links -->
      <div class="flex items-center space-x-8">
        {#each navItems as item}
          <a 
            href={item.href}
            class="text-gray-600 hover:text-gray-900 px-3 py-2 text-sm font-medium transition-colors duration-200 {$page.url.pathname === item.href ? 'text-blue-600 font-semibold' : ''}"
          >
            {item.label}
          </a>
        {/each}
      </div>
    </div>
  </div>
</nav>

<!-- Main content -->
<main class="min-h-screen bg-gray-50">
  <slot />
</main>

<!-- Footer -->
<footer class="bg-white border-t border-gray-200">
  <div class="max-w-4xl mx-auto py-8 px-4 sm:px-6 lg:px-8">
    <div class="text-center text-sm text-gray-500">
      <p>&copy; {new Date().getFullYear()} William Park. Built with SvelteKit & Tailwind CSS.</p>
    </div>
  </div>
</footer> 