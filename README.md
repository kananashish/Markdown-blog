# Markdown Blog

A modern, performant blog built with **Next.js**, styled with **Tailwind CSS** and **Shadcn UI**, and powered by **Pieces** for content management. The blog leverages **Remark** and **Rehype** to process Markdown files, enabling a seamless content creation experience with rich text formatting and dynamic rendering.

## Features
- **Next.js**: Server-side rendering and static site generation for fast, SEO-friendly pages.
- **Shadcn UI**: Beautiful, accessible UI components for a polished user experience.
- **Tailwind CSS**: Utility-first CSS framework for rapid and responsive styling.
- **Pieces**: Efficient content management for organizing and retrieving Markdown-based blog posts.
- **Remark & Rehype**: Robust Markdown processing with support for plugins to handle syntax highlighting, embeds, and more.
- **Responsive Design**: Fully responsive layout optimized for all devices.
- **SEO Optimized**: Metadata and structured data for better search engine visibility.
- **Easy Content Management**: Write blog posts in Markdown and publish effortlessly.

## Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or Yarn
- A Pieces account for content management (optional, depending on setup)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/markdown-blog.git
   cd markdown-blog
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Set up environment variables:
   Create a `.env.local` file in the root directory and add the following:
   ```env
   NEXT_PUBLIC_PIECES_API_KEY=your_pieces_api_key
   ```

4. Run the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```
   Open [http://localhost:3000](http://localhost:3000) to view the blog in your browser.

## Project Structure
```
markdown-blog/
├── content/               # Markdown files for blog posts
├── public/                # Static assets (images, etc.)
├── src/
│   ├── components/        # Reusable Shadcn UI components
│   ├── pages/             # Next.js pages and dynamic routes
│   ├── styles/            # Tailwind CSS and global styles
│   ├── lib/               # Utility functions for Remark/Rehype
├── .env.local             # Environment variables
├── next.config.js         # Next.js configuration
├── tailwind.config.js     # Tailwind CSS configuration
├── README.md              # This file
```

## Writing Posts
1. Create a new Markdown file in the `content/` directory.
2. Use the following frontmatter format for metadata:
   ```markdown
   ---
   title: My Blog Post
   date: 2025-08-05
   author: Your Name
   tags: [tag1, tag2]
   ---
   Your content here...
   ```
3. The post will be automatically processed by Remark and Rehype and rendered on the blog.

## Customization
- **Styling**: Modify `tailwind.config.js` to adjust themes or add custom utilities.
- **Components**: Extend or customize Shadcn UI components in `src/components/`.
- **Markdown Processing**: Add Remark/Rehype plugins in `src/lib/` for features like syntax highlighting or embeds.

## Deployment
Deploy the blog to platforms like Vercel, Netlify, or any Node.js-compatible host:
1. Build the project:
   ```bash
   npm run build
   # or
   yarn build
   ```
2. Deploy using your platform’s CLI or Git integration.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.
