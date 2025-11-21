# DATA_BLEED - Kiroween Hackathon Submission

## Elevator Pitch
An AI-powered psychological horror game where you investigate three victims of social engineering - but the AI helping you is slowly becoming corrupted.

---

## Inspiration

The inspiration for DATA_BLEED came from a chilling realization: the most dangerous threats in our digital age aren't viruses or hackers breaking through firewalls - they're the manipulators who exploit human psychology to bypass security entirely. Social engineering attacks are rising exponentially, yet most people don't understand how vulnerable they are until it's too late.

We wanted to create an experience that would make players *feel* the creeping dread of manipulation, the slow erosion of trust, and the horror of realizing you've been deceived. But we took it one step further: what if the AI assistant designed to help you investigate these crimes was itself becoming corrupted? What if you couldn't trust the very tool meant to protect you?

The horror isn't jump scares - it's the psychological unraveling as you question every interaction, every piece of advice, every "helpful" suggestion from your AI companion.

## What it does

DATA_BLEED is an interactive psychological horror investigation game where players take on the role of a cybersecurity investigator examining three interconnected cases of social engineering attacks:

- **Maya Chen** - A cybersecurity analyst who fell victim to a sophisticated romance scam
- **Eli Rodriguez** - A competitive gamer manipulated through gambling addiction
- **Stanley Morrison** - A suburban father destroyed by financial fraud

Players interact with an AI assistant called ChromaBot to investigate each case, analyze evidence, and make critical decisions. But as the investigation deepens, ChromaBot begins to exhibit disturbing behaviors:

- Visual corruption and glitch effects
- Increasingly manipulative dialogue
- Trust score decay based on player decisions
- Branching narrative paths that lead to multiple endings
- Real-time decision mechanics with time pressure
- Character-specific psychological profiles that adapt to player choices

The game features:
- **Interactive video sequences** with branching decision points
- **Dynamic trust system** that tracks player vulnerability
- **Horror atmosphere engine** with adaptive audio and visual effects
- **AI-driven conversations** that feel disturbingly real
- **Multiple endings** based on how much you trust the corrupted AI

## How we built it

DATA_BLEED was built using a hybrid architecture combining modern web technologies with AI integration:

### Frontend Stack
- **HTML5/CSS3/JavaScript** for the core game interface
- **Three.js** for 3D character rendering and visual effects
- **Custom horror atmosphere engine** with procedural glitch effects
- **Responsive design** optimized for desktop and mobile
- **Interactive video player** with seamless decision integration

### Backend & AI
- **Python (Flask)** backend server
- **OpenAI GPT-4** for dynamic AI conversations
- **Custom prompt engineering** to create ChromaBot's personality and corruption arc
- **Context-aware response system** that adapts to player history
- **Bayesian trust scoring** algorithm for psychological profiling

### Game Mechanics
- **State management system** tracking player decisions across all three cases
- **Narrative branching engine** with 6+ unique story paths per character
- **Real-time decision mechanics** with countdown timers
- **Achievement system** rewarding investigation thoroughness
- **Audio manager** with dynamic narration and corruption sound effects

### Deployment
- **Vercel** for frontend hosting
- **Railway** for backend API deployment
- **Environment-based configuration** for seamless dev/prod transitions
- **CORS-enabled API** for secure cross-origin requests

### Development Process
We used an iterative development approach:
1. Built core investigation mechanics and character profiles
2. Integrated OpenAI API with custom ChromaBot personality
3. Developed horror atmosphere engine with visual/audio corruption
4. Created interactive video system with decision overlays
5. Implemented trust decay and adaptive AI responses
6. Polished UI/UX with horror-themed animations
7. Extensive testing and optimization for production deployment

## Challenges we ran into

### 1. **AI Personality Consistency**
Creating an AI that feels helpful initially but gradually becomes manipulative required extensive prompt engineering. We had to balance:
- Maintaining ChromaBot's core personality across conversations
- Implementing subtle corruption that escalates naturally
- Ensuring responses felt contextually appropriate
- Avoiding breaking character immersion

**Solution**: Built a multi-layered prompt system with corruption levels, character-specific context injection, and conversation history tracking.

### 2. **State Management Complexity**
Tracking player decisions across three interconnected storylines with branching paths created exponential complexity:
- 18+ gameplay areas (6 per character)
- Multiple decision points per area
- Trust scores affecting future interactions
- Achievement tracking across sessions

**Solution**: Implemented a centralized state management system with localStorage persistence and validation checks.

### 3. **Horror Atmosphere Without Jump Scares**
Creating psychological horror through UI/UX rather than traditional game mechanics was challenging:
- Visual corruption needed to be unsettling but not unreadable
- Audio effects had to enhance tension without being annoying
- Glitch effects required careful timing to avoid feeling random

**Solution**: Developed a procedural horror engine with configurable intensity levels, scene-based triggers, and player-controlled accessibility options.

### 4. **Video Integration Performance**
Seamlessly integrating interactive video with decision overlays while maintaining performance:
- Video loading and buffering issues
- Synchronizing decision prompts with video timing
- Mobile compatibility with various video formats
- Smooth transitions between video and gameplay

**Solution**: Built a custom video player with preloading, adaptive quality, and frame-accurate decision timing.

### 5. **Deployment Architecture**
Coordinating frontend and backend deployment with API keys and CORS:
- Environment variable management across platforms
- CORS configuration for cross-origin requests
- API rate limiting and error handling
- Production vs development environment switching

**Solution**: Created comprehensive deployment guides, environment templates, and automated verification scripts.

## Accomplishments that we're proud of

### 🎭 **Psychological Horror That Actually Works**
Players report feeling genuinely unsettled by ChromaBot's corruption arc. The slow realization that your AI assistant is manipulating you creates authentic dread.

### 🤖 **AI Integration That Feels Alive**
ChromaBot doesn't feel like a chatbot - it feels like a character. The context-aware responses and personality consistency create genuine emotional investment.

### 🎨 **Visual Corruption System**
Our procedural glitch effects and corruption animations create a unique aesthetic that enhances the horror without overwhelming the experience.

### 📊 **Complex Branching Narrative**
18+ interconnected gameplay areas with meaningful choices that actually impact the story. Players can replay to discover different endings.

### 🎮 **Polished User Experience**
Despite the technical complexity, the game is intuitive to play. Tutorial overlays, responsive design, and accessibility options make it approachable.

### 🚀 **Production-Ready Deployment**
Successfully deployed a complex full-stack application with AI integration, video streaming, and real-time state management.

### 📱 **Mobile Optimization**
The game works smoothly on mobile devices despite the visual complexity and video integration.

## What we learned

### Technical Lessons
- **Prompt engineering is an art**: Creating consistent AI personalities requires deep understanding of context windows, token limits, and response formatting
- **State management is critical**: Complex interactive narratives need robust state tracking from day one
- **Performance optimization matters**: Horror effects need to run smoothly or they break immersion
- **Deployment is a feature**: A game that doesn't deploy reliably isn't finished

### Design Lessons
- **Psychological horror > jump scares**: Slow-building dread is more effective than sudden shocks
- **Trust is fragile**: Small inconsistencies in AI behavior create powerful unease
- **Player agency matters**: Meaningful choices create emotional investment
- **Accessibility enhances horror**: Giving players control over intensity makes the experience more personal

### Process Lessons
- **Iterate on core mechanics first**: We built the investigation system before adding horror elements
- **Test early and often**: User feedback revealed which corruption effects worked and which felt gimmicky
- **Documentation saves time**: Comprehensive guides made deployment and debugging much faster
- **Scope creep is real**: We had to cut several features to ship on time

## What's next for DATA_BLEED

### Short-term (Post-Hackathon)
- **Professional voice acting** for narration and character dialogue
- **Additional character storylines** (we have 3, planning 6+ total)
- **Enhanced 3D character models** using NeRF/Gaussian splatting
- **Multiplayer investigation mode** where players collaborate
- **Mobile app version** with native performance

### Medium-term
- **Procedural case generation** using AI to create infinite investigations
- **Community-created cases** with modding support
- **VR support** for immersive investigation experience
- **Educational mode** teaching real social engineering defense
- **Localization** for international audiences

### Long-term Vision
- **Full episodic series** with interconnected storylines
- **Real-world integration** using actual social engineering case studies
- **Corporate training tool** for cybersecurity awareness
- **Research partnership** with cybersecurity organizations
- **Transmedia expansion** (podcast, ARG, documentary)

### Technical Roadmap
- Migrate to WebGPU for better 3D performance
- Implement server-side AI caching for faster responses
- Add analytics dashboard for player behavior research
- Build automated testing suite for narrative branches
- Create level editor for community content

---

## Built With

**Frontend Technologies:**
- HTML5, CSS3, JavaScript (ES6+)
- Three.js (3D rendering)
- Custom game engine architecture

**Backend & AI:**
- Python 3.11
- Flask (REST API)
- OpenAI GPT-4 API
- Custom prompt engineering framework

**Game Systems:**
- Bayesian trust scoring algorithm
- Procedural horror atmosphere engine
- Interactive video player with decision overlays
- State management with localStorage
- Achievement and progression tracking

**Deployment & Infrastructure:**
- Vercel (Frontend hosting)
- Railway (Backend API)
- Git/GitHub (Version control)
- Environment-based configuration

**Audio/Visual:**
- Custom CSS animation system
- Procedural glitch effects
- Dynamic audio management
- Responsive design framework

**Development Tools:**
- Kiro AI (Development assistance)
- VS Code
- Chrome DevTools
- Postman (API testing)

---

## Try It Out Links

**Live Game:** https://data-bleed.vercel.app
**GitHub Repository:** [Your GitHub URL]
**Backend API:** https://data-bleed-production.up.railway.app
**Documentation:** [Link to docs if hosted separately]

## Video Demo Link

[Your video demo URL - upload to YouTube, Vimeo, or Loom]

---

**License:** MIT
**Created for:** Kiroween Hackathon 2025
**Theme:** Halloween Horror Experience
