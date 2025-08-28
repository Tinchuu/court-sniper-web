# Court Sniper Web

A modern web application for monitoring badminton court availability and booking information at Auckland Badminton venues.

## Overview

Court Sniper Web is a Next.js TypeScript application that provides real-time visibility into court bookings, availability, and pricing. It's designed to help players quickly find available courts and track booking patterns.

## Features

### Court Availability Dashboard
- **Real-time court status**: Visual grid showing which of the 12 courts are currently free or booked
- **Date selection**: Check availability for any specific date
- **Booking details**: View all bookings with times, rates, and booking types
- **Smart grouping**: Multiple courts booked by the same person/event are displayed as ranges (e.g., "Courts 1-3")

### Advanced Booking Search
- **Date range filtering**: Search bookings across custom time periods
- **Court-specific search**: Filter by individual courts or view all courts
- **Person/Event search**: Find bookings by searching for names or event titles
- **Combined filtering**: Use multiple filters simultaneously for precise results

### Cost Estimation
- **Real-time pricing**: Get accurate cost estimates for booking specific courts and times
- **Duration calculation**: Automatic calculation of booking duration and total costs
- **Account integration**: View account balance and credit availability
- **Multiple court support**: Estimate costs for any of the 12 available courts

## Technical Stack

- **Framework**: Next.js 14 with App Router
- **Language**: TypeScript for type safety
- **Package Manager**: pnpm for efficient dependency management
- **Styling**: Custom CSS with responsive design
- **API Integration**: Server-side API routes to handle external API calls and CORS

## Architecture

The application uses a clean component-based architecture:

- **API Routes**: Server-side proxies handle external API calls to avoid CORS issues
- **Components**: Modular React components for each major feature
- **Type Safety**: Comprehensive TypeScript interfaces for all data structures
- **Responsive Design**: Mobile-friendly interface with CSS Grid and Flexbox

## Data Sources

The application integrates with Auckland Badminton's platform APIs:
- **Booking Feed API**: Retrieves real-time booking data
- **Cost Estimation API**: Provides accurate pricing information

## Getting Started

```bash
# Install dependencies
pnpm install

# Start development server
pnpm dev

# Build for production
pnpm build

# Start production server
pnpm start
```

## Use Cases

- **Players**: Quickly find available courts and check pricing
- **Coaches**: Monitor court usage patterns and plan training sessions
- **Venue Managers**: Track booking trends and court utilization
- **Event Organizers**: Find available courts for tournaments and events

## Court Information

The venue features 12 badminton courts (Court 1-12), each available for booking with different rates depending on time and booking type (casual vs. regular bookings).