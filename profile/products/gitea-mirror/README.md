# Gitea Mirror

<p align="center">
  <img src="https://raw.githubusercontent.com/RayLabsHQ/gitea-mirror/main/.github/assets/logo-no-bg.png" alt="Gitea Mirror Logo" width="120" />
</p>

<p align="center">
  <a href="https://github.com/RayLabsHQ/gitea-mirror/releases/latest"><img src="https://img.shields.io/github/v/tag/RayLabsHQ/gitea-mirror?label=release" alt="release"/></a>
  <a href="https://github.com/RayLabsHQ/gitea-mirror/actions/workflows/astro-build-test.yml"><img src="https://img.shields.io/github/actions/workflow/status/RayLabsHQ/gitea-mirror/astro-build-test.yml?branch=main" alt="build"/></a>
  <a href="https://github.com/RayLabsHQ/gitea-mirror/pkgs/container/gitea-mirror"><img src="https://img.shields.io/badge/ghcr.io-container-blue?logo=github" alt="container"/></a>
  <a href="https://github.com/RayLabsHQ/gitea-mirror/blob/main/LICENSE"><img src="https://img.shields.io/github/license/RayLabsHQ/gitea-mirror" alt="license"/></a>
</p>

> Automatically mirror repositories from GitHub to your self-hosted Gitea instance with a modern, intuitive web interface.

## 🎯 What is Gitea Mirror?

Gitea Mirror is a powerful web application that automates the synchronization of GitHub repositories to your self-hosted Gitea instance. Whether you're backing up your work, creating an offline development environment, or maintaining a private mirror of public repositories, Gitea Mirror handles it all seamlessly.

<p align="center">
  <img src="https://raw.githubusercontent.com/RayLabsHQ/gitea-mirror/main/.github/assets/dashboard.png" alt="Dashboard" width="700" />
</p>

## ✨ Key Features

- **🔁 Comprehensive Mirroring** - Mirror public, private, and starred GitHub repositories
- **🏢 Organization Support** - Mirror entire GitHub organizations with flexible routing strategies
- **🎯 Smart Routing** - Choose between preserving GitHub structure, single organization, or flat user structure
- **⚡ Real-time Dashboard** - Monitor mirror progress with live updates and activity logs
- **🔐 Secure by Design** - JWT authentication with bcrypt password hashing
- **⏱️ Scheduled Mirroring** - Set up automatic periodic synchronization
- **📱 Responsive UI** - Beautiful interface that works on desktop and mobile
- **🐳 Container-Ready** - Multi-arch Docker images for AMD64 and ARM64

## 🚀 Quick Start

Get up and running in under a minute:

```bash
# Clone the repository
git clone https://github.com/RayLabsHQ/gitea-mirror.git
cd gitea-mirror

# Start with Docker Compose
docker compose -f docker-compose.alt.yml up -d

# Access at http://localhost:4321
```

That's it! The first user to sign up becomes the admin. Configure your GitHub and Gitea connections through the intuitive web interface.

## 📸 Screenshots

<table>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/RayLabsHQ/gitea-mirror/main/.github/assets/repositories.png" alt="Repository Management" />
      <p align="center"><i>Repository Management</i></p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/RayLabsHQ/gitea-mirror/main/.github/assets/organisation.png" alt="Organization Overview" />
      <p align="center"><i>Organization Overview</i></p>
    </td>
  </tr>
</table>

## 🏗️ Architecture

Built with modern web technologies for performance and developer experience:

- **Frontend**: Astro (SSR) + React + Tailwind CSS v4 + Shadcn UI
- **Backend**: Bun runtime for blazing fast performance
- **Database**: SQLite with Drizzle ORM
- **APIs**: GitHub API (Octokit) and Gitea REST API
- **Real-time**: Server-Sent Events for live updates

## 🔧 Installation Options

### Docker (Recommended)
- Pre-built multi-arch images on GitHub Container Registry
- Simple docker-compose setup with sensible defaults
- Automatic database initialization

### Proxmox VE
- One-line LXC container installation script
- Part of the Proxmox VE Community Scripts collection

### Manual Installation
- Requires Bun runtime
- Ideal for development and customization

## 🤝 Contributing

We welcome contributions! Whether it's bug fixes, new features, or documentation improvements, check out our [Contributing Guidelines](https://github.com/RayLabsHQ/gitea-mirror/blob/main/CONTRIBUTING.md).

## 📚 Resources

- 📖 [Full Documentation](https://github.com/RayLabsHQ/gitea-mirror)
- 🐛 [Report Issues](https://github.com/RayLabsHQ/gitea-mirror/issues)
- 💬 [Join Discussions](https://github.com/RayLabsHQ/gitea-mirror/discussions)
- 🔧 [Proxmox VE Script](https://community-scripts.github.io/ProxmoxVE/scripts?id=gitea-mirror)

## 📄 License

GNU General Public License v3.0 - see [LICENSE](https://github.com/RayLabsHQ/gitea-mirror/blob/main/LICENSE) for details.

---

<p align="center">Made with ❤️ by <a href="https://github.com/RayLabsHQ">RayLabs</a></p>