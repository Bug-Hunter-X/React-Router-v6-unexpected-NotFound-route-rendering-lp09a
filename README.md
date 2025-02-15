# React Router v6 NotFound Route Issue

This repository demonstrates a problem with the catch-all route ("*" path) in React Router v6.  The NotFound component is rendering even when a valid route is available.

## Problem Description:
When navigating between valid routes, the NotFound component renders unexpectedly, interfering with the expected application flow.

## Solution:
The issue is resolved by ensuring all other routes are specified *before* the catch-all route.  This ensures that the catch-all route only matches when no other route matches the URL.