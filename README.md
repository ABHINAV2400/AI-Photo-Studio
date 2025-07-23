# AI Photo Studio 🎨✨

**A full-stack AI-powered photo editor built with Next.js, Fabric.js, Tailwind CSS, Convex, Clerk, and ImageKit.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

## 🌟 Overview

AI Photo Studio is a powerful, user-friendly photo editing application that leverages the latest in web technologies and artificial intelligence. This application allows users to upload, edit, and enhance their photos with a variety of tools and AI-powered features. The frontend is built with **Next.js** for a fast and responsive user experience, while **Fabric.js** provides a flexible and interactive canvas for image manipulation.

This project integrates a full suite of modern tools to deliver a seamless experience from user authentication to cloud-based image storage.

## ✨ Features

* **User Authentication**: Secure user sign-up and sign-in functionality powered by **Clerk**.
* **Image Upload**: Upload images from your local machine to the editor.
* **Interactive Canvas**: A dynamic and responsive editing canvas built with **Fabric.js**.
* **Rich Image Editing Tools**:
    * Add and customize text.
    * Draw freeform lines and shapes.
    * Insert various shapes (circles, rectangles, triangles).
    * Apply image filters (e.g., grayscale, sepia).
    * Remove objects from the image.
* **AI-Powered Capabilities**:
    * **AI Image Filling**: Intelligently fill parts of an image.
    * **Background Removal**: Automatically remove the background from photos.
* **Image & Metadata Storage**: Seamlessly save, manage, and retrieve edited photos and their metadata with **Convex** as the backend.
* **Cloud Media Management**: Efficiently handle image transformations and delivery via **ImageKit**.
* **Utility Features**:
    * Undo/Redo functionality.
    * Download edited images.
    * View and manage a gallery of created images.

## 🚀 Tech Stack

### Frontend

* **Framework**: [Next.js](https://nextjs.org/)
* **UI Components**: [Shadcn UI](https://ui.shadcn.com/)
* **Canvas Library**: [Fabric.js](http://fabricjs.com/)
* **Styling**: [Tailwind CSS](https://tailwindcss.com/)
* **Icons**: [Lucide React](https://lucide.dev/)

### Backend & Infrastructure

* **Backend & Database**: [Convex](https://www.convex.dev/) (Real-time backend for an application state)
* **Authentication**: [Clerk](https://clerk.com/)
* **Image Management & Storage**: [ImageKit](https://imagekit.io/)
* **Image Search**: [Unsplash API](https://unsplash.com/developers)

## 🛠️ Getting Started

Follow these instructions to get a local copy of the project up and running for development and testing purposes.

### Prerequisites

* Node.js (v18 or later)
* npm, yarn, or pnpm

### Installation

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/ABHINAV2400/AI-Photo-Studio.git](https://github.com/ABHINAV2400/AI-Photo-Studio.git)
    cd AI-Photo-Studio
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    # or
    yarn install
    ```

3.  **Set up Convex:**

    You need to have the Convex CLI installed and be logged in.

    ```bash
    npm install -g convex
    convex login
    ```

4.  **Set up environment variables:**

    Create a `.env` file in the root of your project and add the following variables. You can obtain these keys from the respective service dashboards.

    ```env
    # Deployment used by `npx convex dev`
    CONVEX_DEPLOYMENT=

    # Get from Convex project settings
    NEXT_PUBLIC_CONVEX_URL=

    # Get from Clerk dashboard
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=
    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

    # This should be your Clerk project's JWT issuer domain
    # e.g., [https://your-domain.clerk.accounts.dev](https://your-domain.clerk.accounts.dev)
    CLERK_JWT_ISSUER_DOMAIN=

    # Get from ImageKit dashboard
    NEXT_PUBLIC_IMAGEKIT_PUBLIC_KEY=
    NEXT_PUBLIC_IMAGEKIT_URL_ENDPOINT=
    IMAGEKIT_PRIVATE_KEY=

    # Get from Unsplash Developer portal
    NEXT_PUBLIC_UNSPLASH_ACCESS_KEY=
    ```

5.  **Run the development server:**

    In one terminal, run the Convex development server:
    ```bash
    npx convex dev
    ```

    In another terminal, run the Next.js application:
    ```bash
    npm run dev
    ```

    Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📜 License

Distributed under the MIT License. See `LICENSE.txt` for more information.
