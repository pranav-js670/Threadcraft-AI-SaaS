# Threadcraft AI

Welcome to **Threadcraft AI**, a powerful AI-driven SaaS platform that generates optimized social media content for Twitter, Instagram, and LinkedIn. Built for content creators, marketers, and businesses, Threadcraft AI helps craft compelling Twitter threads, Instagram captions, and LinkedIn posts, all powered by cutting-edge AI technology.

## Features

- **AI-Powered Content Generation**: Leveraging Google's **Gemini AI** for generating high-quality and engaging content across three platforms.
  - **Twitter**: Generate detailed and insightful Twitter threads.
  - **Instagram**: Create captivating Instagram captions to boost engagement.
  - **LinkedIn**: Write professional and thought-provoking LinkedIn posts.
  
- **Next.js Framework**: Optimized for fast performance and SEO with the power of Next.js.
  
- **ShadCN UI Components**: Clean, accessible, and responsive UI elements, styled with Tailwind CSS.
  
- **Backend with Supabase & Neon**: Scalable and secure data management powered by Supabase as a database and Neon for efficient PostgreSQL support.

- **Seamless Stripe Integration**: Monetize your SaaS with Stripe for payments and subscriptions.

## 🛠️ Tech Stack

- **Frontend**: Next.js 14, React 18, Tailwind CSS, ShadCN UI
- **Backend**: Supabase, Neon, Drizzle ORM
- **AI Integration**: Google's **Gemini AI**
- **Payments**: Stripe
- **UI Components**: Radix UI, Tailwind Merge
- **Database**: PostgreSQL with Supabase & Neon

## 🚀 Getting Started

To get started with Threadcraft AI, follow these steps:

### Prerequisites

Make sure you have the following installed:
- [Node.js](https://nodejs.org/en/download/) (v18+)
- [PostgreSQL](https://www.postgresql.org/download/) or use **Supabase** for database management.
- [Stripe Account](https://stripe.com/) for payment gateway integration.

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/<your-username>/ThreadcraftAI-SocialMedia-Content-Generator.git
    ```
    
2. **Navigate to the project directory**:
    ```bash
    cd ThreadcraftAI-SocialMedia-Content-Generator
    ```

3. **Install dependencies**:
    ```bash
    npm install
    ```

4. **Set up environment variables**:
   Create a `.env.local` file in the root of your project with the following variables:
   
    ```bash
    NEXT_PUBLIC_SUPABASE_URL=<your_supabase_url>
    NEXT_PUBLIC_SUPABASE_ANON_KEY=<your_supabase_anon_key>
    DATABASE_URL=<your_neon_postgres_url>
    STRIPE_SECRET_KEY=<your_stripe_secret_key>
    GEMINI_API_KEY=<your_google_gemini_api_key>
    ```

5. **Start the development server**:
    ```bash
    npm run dev
    ```

6. **Run database migrations**:
    Use Drizzle ORM to manage your database schema:
    ```bash
    drizzle-kit migrate:run
    ```

### Using Ngrok for Stripe Webhooks

If you're running the app locally and want to test Stripe payments, you'll need to expose your local environment to a public URL. Use ngrok to create a tunnel:

1. Install ngrok:
    ```bash
    npm install -g ngrok
    ```

2. Run ngrok:
    ```bash
    ngrok http 3000
    ```

3. Update your Stripe webhook settings with the ngrok-generated public URL.


## Contact

For any questions or issues, feel free to reach out:

- **Email**: [jspranav15@gmail.com](mailto:jspranav15@gmail.com)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
