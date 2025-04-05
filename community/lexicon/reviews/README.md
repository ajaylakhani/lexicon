# Reviews Lexicon

A standardized schema for user-generated reviews across various domains within the atproto ecosystem.

## Overview

This lexicon provides a flexible yet structured way to represent reviews for different types of entities, including products, services, locations, media, and experiences. It aims to create a consistent format that can be used across various applications while allowing for domain-specific details.

## Key Features

- **Versatile subject identification** - Review any entity with a URI
- **Standardized rating system** - Consistent 1-5 rating scale
- **Rich media support** - Attach images and videos with accessibility information
- **Detailed metrics** - Domain-specific rating breakdowns
- **Trust mechanisms** - Verified purchase indicators, disclosure flags
- **Licensing controls** - Specify how review content can be used and shared
- **Syndication permissions** - Allow or disallow sharing across platforms

## Usage

### Basic Required Fields

The minimal valid review requires only:
- `subject` - What is being reviewed (with type and URI)
- `rating` - A numerical rating from 1-5
- `createdAt` - When the review was created

### Optional Enhancements

The schema supports many optional fields including:
- `content` - Detailed review text
- `media` - Images or videos with alt text
- `metrics` - Specific ratings for different aspects
- `categories` - Tags for categorization
- And many more

## Examples

This repository includes example JSON files for various review types:
- [Book Review](./examples/book-review.json)
- [Movie Review](./examples/movie-review.json)
- [Product Review](./examples/product-review.json)
- [Service Review](./examples/service-review.json)
- [Location Review](./examples/location-review.json)

## Integration

To integrate with this lexicon in your application:

1. Use `community.lexicon.reviews.main` as the record type
2. Ensure required fields are included
3. Add optional fields as needed for your specific use case

## Contributing

Feedback and contributions to this lexicon are welcome. Please follow the standard Lexicon Community contribution guidelines outlined in the [Contributor Guide](../../CONTRIBUTING.md).