# QingIcon

QingIcon is a **standardized, neutral-style** UI icon set — free and open source (Apache 2.0), built for AI, cloud, and internet products. Every icon shares the same grid and visual weight, so they mix cleanly without clashing.

- **3900+ icons** across **34 categories**;
- Two styles: **Line** and **Fill** (fill variants are still being drawn);
- **137,235 bilingual (Chinese + English) keywords** for high recall — "if you can think of it, you can usually find it";
- Browse, search, copy, and download on the website; also available as React / Vue components, an MCP Server, and a Figma plugin.
- Website: https://qingicon.com



## Core Capabilities

### Neutral, consistent visual language
Uniform sizing and balanced visual weight — icons obey their own law of conservation of energy.

### Sketch style
One click switches any icon into a hand-drawn sketch look (the irregularity and warmth of a quick sketch), turning an engineering feel into a "human is thinking" vibe. Great for concept drafts, wireframes, brainstorming, teaching, and proposals. The same icon flips instantly and losslessly between "neutral" and "sketch" — fully interchangeable.

> The sketch style is a **website and Figma plugin** design-side feature. It is **not** shipped in the npm component packages or the MCP. If you want this capability in your own build, you can bring in [Rough.js](https://roughjs.com/) yourself.

### Chinese & English search
137k+ bilingual keywords, backed by a lot of engineering polish:

- **Chinese segmentation + fuzzy tolerance**: tokenizes Chinese with the browser-native `Intl.Segmenter` — no-space Chinese is auto-segmented and matched on multi-term AND; fragments still resolve. Typing `早蛋` (only half-remembered) still recalls icons containing both `早餐` (breakfast) and `鸡蛋` (egg).
- **English side**: normalization (`userpen`→`user-pen`), order-independence (`pen user`→`user-pen`), and fuzzy fallback (`pecil`→`pencil`).

### Abstract icons (the always-available fallback library)
The in-library **Abstract** category is semantically broad and endlessly reusable. When a concrete icon doesn't fit a feature, an abstract icon is the universal stand-in — drop it in as a container / marker / decoration / placeholder so the screen is never empty. That's exactly why the abstract set is large, comprehensive, and still growing: it's the library's safety net.

### Cloud / AI scenarios
Built out systematically by product domain, specifically for AI, cloud, and internet products:

- **AI icons**: the full AI product chain — models, inference, training, Agents, neural networks, vectors, prompts, conversation, and more.
- **Cloud / network icons**: servers, databases, containers, networking, storage, CDN, monitoring — all the cloud-native / cloud-service primitives you need for cloud architecture diagrams, cloud consoles, and SaaS dashboards.
- These families share the same neutral grid as the rest of the UI icons, so they never fight when mixed — **a single QingIcon covers the entire "AI + cloud" product surface**, no need to stitch together three or four mismatched icon sources.

### Optical correction
Keeps stroke visual weight consistent when scaling, avoiding the distortion where lines look thick at small sizes and thin at large sizes.

### Padlock cross-tool placeholder
Exports include an invisible square boundary layer (`fill=none stroke=none`) so external tools like Sketch / Figma preserve the icon's canvas size consistently across tools.

### Multi-format export
Tune stroke, size, and color live on the website. One-click copy of **SVG / React / Vue / DataURL**, plus download of **SVG / PNG / WebP**; more export formats are coming.



## Why this project

I'd long been frustrated with most icon libraries: inconsistent sizing, unbalanced visual weight, and a lack of versatile abstract icons for diverse scenarios. In an age where AI is everywhere, I decided to settle down and craft some foundational design services — to distill a designer's proudest work. That's how this project began.



## Ecosystem

| Ecosystem | Description | Link |
|---|---|---|
| **Website** | Browse / search / copy / download online | https://qingicon.com |
| **React component** `qingicon-react` | One `Qi{Name}` component per icon, with Tree-shaking, TypeScript, and Optical | [npm](https://www.npmjs.com/package/qingicon-react) |
| **Vue component** `qingicon-vue` | Same, as Vue 3 components | [npm](https://www.npmjs.com/package/qingicon-vue) |
| **MCP Server** `qingicon-mcp` | Search or look up matching icons in natural language from AI coding tools (Cursor, Claude Code, Codex, VS Code Copilot, etc.), generating paste-ready React / Vue component code or inline HTML SVG | [npm](https://www.npmjs.com/package/qingicon-mcp) |
| **Figma plugin** | Bring the icon library into Figma | https://www.figma.com/community/plugin/1686396239772536401 |



## Collaboration & Feedback

We welcome **icon requests, bug reports, and keyword contributions**:

- **Open an Issue**: preferred — easy to track and discuss with the community
- **WeChat group or Slack channel**: see the website
- **Email**: cjl294114430@gmail.com or asornch@gmail.com

Whether you want a specific icon, found a rendering or search problem, or want to add keywords for an icon, reach out through any of the above.



## Author

**Asorn** (Design & Vibecoding)

- Blog: https://asorn.cn

This is a purely non-profit project, and maintaining it is genuinely hard work. If you'd like, please give us a Star, or sponsor the project on the website.



## License

Released under **Apache 2.0**: free for personal and commercial use, modifiable and redistributable, provided the license notice is retained; no express warranty. Full terms at https://www.apache.org/licenses/LICENSE-2.0 or the `LICENSE` file in this repo.
