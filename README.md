# QuizAPI

QuizAPI (https://quizapi.io/) gives developers programmatic access to thousands of quiz questions across topics such as programming, science, mathematics, and general knowledge. The service is designed for trivia apps, learning and assessment platforms, embedded quizzes, and gamified onboarding flows. Questions can be filtered by category, difficulty, and tags, and full quizzes can be created, retrieved, and populated with questions through a JSON REST API.

## QuizAPI REST API

The QuizAPI REST API exposes a focused set of endpoints for content discovery, quiz management, and question retrieval. All requests are JSON and authenticated with a Bearer API key (`Authorization: Bearer qz_live_...`) issued from the QuizAPI dashboard. Responses follow a consistent `data` / `meta` envelope and support pagination via `page` and `per_page` parameters.

**Base URL:** `https://quizapi.io`

### Endpoints

- `GET /api/v1/metadata` - Retrieve API metadata, supported difficulties, and global counts.
- `GET /api/v1/categories` - List quiz categories.
- `GET /api/v1/quizzes` - Browse and search published quizzes.
- `POST /api/v1/quizzes` - Create a new quiz.
- `GET /api/v1/quizzes/{id}` - Retrieve a specific quiz.
- `GET /api/v1/questions` - Retrieve questions across quizzes with filtering.
- `POST /api/v1/quizzes/{id}/questions/batch` - Batch-import questions into a quiz.

### API Resources

- **Documentation:** https://quizapi.io/docs
- **Authentication:** https://quizapi.io/docs/authentication
- **Rate Limits:** https://quizapi.io/docs/rate-limits
- **Webhooks:** https://quizapi.io/docs/webhooks
- **SDKs:** https://quizapi.io/docs/sdks
- **Sign Up:** https://quizapi.io/signup

## OpenAPI Specification

The official OpenAPI 3.1 specification published by QuizAPI has been mirrored into this repository:

- **Upstream OpenAPI:** https://quizapi.io/api/v1/openapi.json
- **Local OpenAPI:** [openapi/quiz-api-openapi.json](openapi/quiz-api-openapi.json)

## Links

- **Website:** https://quizapi.io/
- **Documentation:** https://quizapi.io/docs
- **Support / Issues:** https://github.com/QuizAPI/support/issues

## Maintainers

- **FN:** Kin Lane
- **Email:** kin@apievangelist.com
