# Forge

Design for a Windows desktop studio that builds an AI workflow by dragging tools onto a canvas and running it locally.

## Problem

Skills, plugins, and connected tools already exist on the machine. A dashboard cannot wire them together. The goal is a canvas: drop a tool, connect success and error paths, press Run, and watch each step.

## What the design specifies

- Electron app with an infinite canvas
- Catalog of local skills, plugins, and tool servers, plus ordinary nodes such as HTTP, files, and branches
- Drag onto the canvas, connect success and error handles, run the graph on this machine
- Per-node status and a run log
- Hover help on each object
- Save and load workflows

Run is manual. The v1 design leaves out schedules, webhooks, and multi-user hosting.

## Stack

Electron, a Vite renderer, a node canvas, TypeScript, local tool adapters.

## Status

Private design and implementation plan. The desktop app is not built yet. This page does not include machine paths or credentials.
