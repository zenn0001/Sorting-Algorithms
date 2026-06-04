# Sorting Algorithms Visualizer 🎱

A modern, interactive web application for visualizing and comparing sorting algorithms. This project provides step-by-step visual demonstrations of how different sorting algorithms work, complete with performance metrics, code examples, and side-by-side comparisons.

## 🎯 Features

- **Interactive Visualizations**: Watch sorting algorithms work in real-time with animated bar charts
- **Three Core Algorithms**: Bubble Sort, Merge Sort, and Quick Sort
- **Detailed Algorithm Pages**: Learn about each algorithm with:
  - Step-by-step visualization with color-coded indicators
  - Real-time comparison and swap counters
  - Time and space complexity information
  - Full source code with syntax highlighting
  - Algorithm descriptions and use cases
- **Algorithm Comparison**: View all three algorithms sorting the same array simultaneously to understand performance differences
- **Complexity Analysis**: Visual complexity graphs showing O(n) performance characteristics
- **Adjustable Controls**:
  - Playback speed control (from slow to fast)
  - Array size adjustment
  - Random array generation
  - Step-by-step navigation
- **Sound Effects**: Optional audio feedback for sorting operations
- **Responsive Design**: Works seamlessly on desktop and tablet devices
- **Smooth Animations**: Framer Motion-powered transitions and visual effects

## 🛠️ Tech Stack

- **Framework**: [Next.js](https://nextjs.org/) 16.2.6
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **UI Components**: React 18.2.0
- **Rendering**: Canvas API for efficient visualizations

## 📁 Project Structure

```
├── app/                           # Next.js app directory
│   ├── page.tsx                   # Home page with algorithm cards
│   ├── bubble-sort/               # Bubble Sort page
│   ├── merge-sort/                # Merge Sort page
│   ├── quick-sort/                # Quick Sort page
│   ├── compare/                   # Side-by-side comparison page
│   └── globals.css                # Global styles
├── components/                    # Reusable React components
│   ├── AlgoCard.tsx               # Algorithm card component
│   ├── AlgoDescription.tsx        # Algorithm description panel
│   ├── AlgorithmPage.tsx          # Main algorithm page layout
│   ├── CodePanel.tsx              # Source code display
│   ├── CompareVisualizer.tsx      # Multi-algorithm visualizer
│   ├── ComplexityCard.tsx         # Complexity information display
│   ├── ComplexityGraph.tsx        # Big-O complexity visualization
│   ├── Controls.tsx               # Playback and array controls
│   ├── Visualizer.tsx             # Canvas-based bar chart visualizer
│   ├── NavBar.tsx                 # Navigation header
│   ├── PageSkeleton.tsx           # Loading skeleton
│   ├── PageTransition.tsx         # Page transition effects
│   └── SoundProvider.tsx          # Sound context provider
├── lib/                           # Utility functions and types
│   ├── algoInfo.ts                # Algorithm information & code snippets
│   ├── bubbleSort.ts              # Bubble sort implementation
│   ├── mergeSort.ts               # Merge sort implementation
│   ├── quickSort.ts               # Quick sort implementation
│   ├── arrayUtils.ts              # Array utilities (random generation)
│   ├── sounds.ts                  # Sound effects engine
│   └── types.ts                   # TypeScript type definitions
├── public/                        # Static assets
├── package.json                   # Dependencies and scripts
├── tsconfig.json                  # TypeScript configuration
├── next.config.js                 # Next.js configuration
├── tailwind.config.ts             # Tailwind CSS configuration
└── postcss.config.js              # PostCSS configuration
```

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ or later
- npm, yarn, pnpm, or bun

### Installation

1. Clone the repository:
```bash
git clone https://github.com/JerichoDelosReyes/Sorting-Algorithms.git
cd Sorting-Algorithms
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Open your browser and navigate to:
```
http://localhost:3000
```

## 📖 Usage

### Home Page
The landing page displays three algorithm cards:
- **Bubble Sort**: A simple comparison-based algorithm
- **Merge Sort**: A divide-and-conquer approach
- **Quick Sort**: An efficient partitioning-based algorithm

Click on any card to navigate to its detailed visualization page.

### Algorithm Pages
Each algorithm page includes:
- **Visualizer**: Canvas-based animated visualization showing array sorting
- **Controls**: Play/pause, speed adjustment, array size control, and step navigation
- **Metrics**: Real-time display of comparisons and swaps performed
- **Description**: Detailed explanation of how the algorithm works
- **Code Panel**: Full source code implementation with syntax highlighting
- **Complexity Card**: Time and space complexity information

### Compare Page
Navigate to the Compare section to see all three algorithms working on the same random array simultaneously. This helps visualize the performance differences between algorithms.

## 🎨 Visual Indicators

The visualizer uses color-coded bars to indicate different states:
- **Gray**: Default/inactive bars
- **Blue**: Currently comparing elements
- **Red**: Elements being swapped
- **Yellow/Orange**: Pivot element (Quick Sort)
- **Purple**: Elements being merged (Merge Sort)
- **Green**: Elements in final sorted position

## ⚙️ Scripts

```bash
npm run dev      # Start development server with hot reload
npm run build    # Build for production
npm start        # Start production server
```

## 🎓 Learning Outcomes

This project helps understand:
- How sorting algorithms work step-by-step
- Time complexity analysis (Big-O notation)
- Space complexity considerations
- Performance comparison between different approaches
- Visual algorithm animation techniques
- Canvas API for efficient rendering
- React hooks and state management
- TypeScript for type-safe development

## 📊 Supported Algorithms

### Bubble Sort
- **Time Complexity**: O(n²) average and worst case, O(n) best case
- **Space Complexity**: O(1)
- **Description**: Repeatedly steps through the array, compares adjacent elements, and swaps them if they're in the wrong order

### Merge Sort
- **Time Complexity**: O(n log n) all cases
- **Space Complexity**: O(n)
- **Description**: Divide-and-conquer algorithm that divides the array into halves, recursively sorts them, and merges the sorted halves

### Quick Sort
- **Time Complexity**: O(n log n) average case, O(n²) worst case
- **Space Complexity**: O(log n) due to recursion
- **Description**: Divide-and-conquer algorithm that partitions the array around a pivot element and recursively sorts the partitions

## 🔊 Audio Features

The application includes optional sound effects to provide audio feedback during the sorting process. Users can toggle sound on/off via the UI.

## 🎯 Future Enhancements

Potential features for future versions:
- Additional sorting algorithms (Heap Sort, Shell Sort, Counting Sort, etc.)
- Algorithm difficulty level selection
- Custom array input
- Code playback with line highlighting
- Performance benchmarking tools
- Algorithm variant comparisons
- Tutorial mode with guided lessons
- Dark mode theme

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📧 Contact

For questions or feedback, please visit the [GitHub repository](https://github.com/JerichoDelosReyes/Sorting-Algorithms).

---

**Happy Sorting! 🚀**
