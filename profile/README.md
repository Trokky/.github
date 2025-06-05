# Trokky CMS 
## Modern Content Management, Your Way

<div align="center">

[![GitHub Stars](https://img.shields.io/github/stars/Trokky?style=social)](https://github.com/Trokky)
[![NPM Downloads](https://img.shields.io/npm/dm/@trokky/create-project)](https://npmjs.com/package/@trokky/create-project)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Discord](https://img.shields.io/badge/chat-discord-7289da.svg)](https://discord.gg/trokky)

**Build content-driven applications with the flexibility of code and the power of modern tooling**

[Get Started](#quick-start) • [Documentation](https://docs.trokky.com) • [Community](https://discord.gg/trokky) • [Issues](https://github.com/Trokky/trokky/issues)

</div>

---

## Choose Your Trokky

We offer **two distinct products** to match your project needs:

<table>
<tr>
<td width="50%" align="center">

### **Trokky Pro**
*Modern • Composable • Enterprise*

```bash
npx @trokky/create-project my-cms
```

**Perfect for:**
- Enterprise applications
- Custom framework needs
- Scalable architectures
- Modern development

[**Explore Trokky Pro**](https://github.com/Trokky/trokky)

</td>
<td width="50%" align="center">

### **Trokky Classic**
*Stable • Simple • Reliable*

```bash
npm install trokky-classic
```

**Perfect for:**
- Quick prototypes
- Small-medium projects  
- Simple requirements
- Proven stability

[**Explore Trokky Classic**](https://github.com/Trokky/trokky-classic)

</td>
</tr>
</table>

---

## Quick Start

### For Modern Projects (Recommended)
```bash
# Create a new Trokky Pro project
npx @trokky/create-project my-blog --template=blog-express --dev

# Navigate and start
cd my-blog
npm run dev
```

### For Simple Projects
```bash
# Install Trokky Classic
npm install trokky-classic

# Quick setup
npx trokky-classic init my-site
cd my-site && npm run dev
```

---

## Why Developers Choose Trokky

<div align="center">

| **Schema-Driven** | **Framework Agnostic** | **Git Native** | **Modern Admin** |
|:---:|:---:|:---:|:---:|
| Define content with TypeScript schemas | Works with Express, Fastify, Koa | Version control your content | React-based interface |

</div>

### Core Features
- **Type-Safe Schemas** - Define content models with full TypeScript support
- **File-Based Storage** - Content stored as JSON files with Git integration
- **GraphQL & REST APIs** - Auto-generated APIs from your schemas
- **Admin Interface** - Modern React-based content management
- **Framework Flexibility** - Use with any Node.js framework
- **Developer Experience** - Hot reloading, TypeScript, modern tooling

---

## Built for Every Scale

<table>
<tr>
<td align="center">

### **Startups**
Quick prototypes and MVPs
<br>
*Use Trokky Classic*

</td>
<td align="center">

### **Enterprises**
Scalable, composable architecture
<br>
*Use Trokky Pro*

</td>
<td align="center">

### **Agencies**
Client projects with flexibility
<br>
*Choose based on scope*

</td>
</tr>
</table>

---

## Example: Blog in 2 Minutes

```typescript
// content/schemas/post.ts
import { schema, string, text, date, image } from '@trokky/schema-builder';

export default schema('post')
  .title('Blog Post')
  .field(string('title').required())
  .field(text('content').required())
  .field(image('featuredImage').optional())
  .field(date('publishDate').defaultToToday())
  .build();
```

```graphql
# Auto-generated GraphQL API
query {
  allPosts {
    nodes {
      title
      content
      featuredImage { url }
      publishDate
    }
  }
}
```

**Result**: Fully functional CMS with admin interface, APIs, and type safety.

---

## Our Repositories

### Featured Projects

<table>
<tr>
<td>

**[Trokky Pro](https://github.com/Trokky/trokky)**
<br>Modern, composable CMS architecture
<br>![Stars](https://img.shields.io/github/stars/Trokky/trokky?style=social)

</td>
<td>

**[Trokky Classic](https://github.com/Trokky/trokky-classic)**
<br>Stable, monolithic CMS for quick setup
<br>![Stars](https://img.shields.io/github/stars/Trokky/trokky-classic?style=social)

</td>
</tr>
</table>

### Tools & Extensions
- **[@trokky/create-project](https://npmjs.com/package/@trokky/create-project)** - Modern CLI for project scaffolding
- **[@trokky/migrate](https://npmjs.com/package/@trokky/migrate)** - Migration tools between versions
- **[Trokky VS Code Extension](https://marketplace.visualstudio.com/items?itemName=trokky.vscode)** - Enhanced development experience

---

## Community & Support

<div align="center">

### Join Our Community

[![Discord](https://img.shields.io/badge/Discord-Join%20Server-7289da?style=for-the-badge&logo=discord)](https://discord.gg/trokky)
[![Twitter](https://img.shields.io/badge/Twitter-Follow-1da1f2?style=for-the-badge&logo=twitter)](https://twitter.com/TrokkyCMS)
[![GitHub](https://img.shields.io/badge/GitHub-Star-181717?style=for-the-badge&logo=github)](https://github.com/Trokky)

### Resources

[Documentation](https://docs.trokky.com) • [Tutorials](https://docs.trokky.com/tutorials) • [Examples](https://github.com/Trokky/examples) • [Support](https://github.com/Trokky/trokky/discussions)

</div>

---

## Contributing

We welcome contributions to all Trokky projects! Here's how you can help:

- **Report bugs** in our [issue trackers](https://github.com/Trokky/trokky/issues)
- **Suggest features** in [discussions](https://github.com/Trokky/trokky/discussions)
- **Improve documentation** with pull requests
- **Contribute code** following our [contribution guidelines](https://docs.trokky.com/contributing)

### Core Team
- **[@amenophis1er](https://github.com/amenophis1er)** - Creator & Lead Developer
- **[@TrokkyTeam](https://github.com/TrokkyTeam)** - Core Contributors

---

## Roadmap

### Current Focus
- Trokky Pro composable architecture
- Core export implementations
- Enhanced CLI experience

### Coming Soon
- Plugin system
- Real-time collaboration
- Enhanced media processing
- Multi-language support

### Future Vision
- Cloud integrations
- Advanced workflow management
- Enterprise features
- Mobile SDKs

---

## Statistics

<div align="center">

![GitHub Org's stars](https://img.shields.io/github/stars/Trokky?style=social)
![GitHub followers](https://img.shields.io/github/followers/Trokky?style=social)
![NPM Downloads](https://img.shields.io/npm/dt/@trokky/create-project)

**Trusted by developers worldwide**

</div>

---

<div align="center">

### **Ready to Build Something Amazing?**

Choose your path and start building with Trokky today!

[**Get Started with Trokky Pro**](https://github.com/Trokky/trokky) • [**Try Trokky Classic**](https://github.com/Trokky/trokky-classic)

---

*Built with care by the Trokky Team*

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

</div>