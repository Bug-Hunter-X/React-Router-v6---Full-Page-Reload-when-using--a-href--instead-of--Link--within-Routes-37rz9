# React Router v6 - Unexpected Full Page Reload with Anchor Tags inside Routes

This repository demonstrates a common issue encountered when using React Router v6:  incorrectly employing `<a href>` tags instead of `<Link>` components within route components.  This leads to unintended full page reloads, bypassing React Router's client-side routing capabilities.

## Problem

Using `<a href>` within routes (as opposed to `<Link>`) causes the browser to perform a full page reload, ignoring the React Router's routing logic.  This is suboptimal as it hinders the single-page application (SPA) experience.

## Solution

Always utilize the `<Link>` component from `react-router-dom` for navigation within your React Router application.  The `<Link>` component interacts with React Router to manage client-side routing effectively.