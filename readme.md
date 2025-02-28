# Dynamic Posts Loader

## Overview
This project demonstrates an efficient approach to loading and displaying content dynamically without continuously adding DOM elements to the page. Instead of creating new elements for each batch of loaded content, this application reuses a fixed set of containers, updating only their content.

## Features
- Displays posts with author names and text content
- Loads content in batches (5 posts at a time)
- Navigation buttons to jump to the beginning or load more content
- Smooth infinite scrolling implementation:
  - Load next page when scrolling down
  - Load previous page when scrolling up
- Performance optimized by reusing DOM elements instead of creating new ones
- Visual feedback with loading animation and smooth transitions

## How It Works
1. The application creates a fixed number of post containers (5) at initialization.
2. When new content is requested, existing containers are updated with new data.
3. Navigation state is managed to keep track of current position in the content.
4. Smart scroll detection prevents interference between user scrolling and programmatic scrolling.

## Technical Highlights
- Pure JavaScript without external dependencies
- CSS animations for smooth transitions
- Fixed navigation header with page indicators
- Efficient DOM manipulation techniques
- Scroll position management to maintain natural scrolling experience

## Usage
Simply open `index.html` in your web browser. No server or build process required!

This demo includes 50 sample posts generated automatically, but the same approach can be used with API data from a real backend.

## Why This Approach?
Traditional infinite scrolling implementations often append new elements to the DOM indefinitely, which can cause performance issues as the page grows. This implementation demonstrates how to achieve the same user experience while maintaining a small DOM footprint.