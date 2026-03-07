# Contributing to Awesome-Action-Chunking

Thank you for contributing to this curated list. Contributions are welcome to keep this repository accurate and useful.

## How to Add a Paper

1. Fork this repository.
2. Edit `README.md` and add the paper in the appropriate section.
3. Submit a Pull Request with a short and clear description.

### Paper Entry Format

Use this table format:

```markdown
| [Paper Title](https://arxiv.org/abs/XXXX.XXXXX) | Method Name | YYYY/MM | Domain/Task | [Code](https://github.com/...) | Venue |
```

Required fields:

- Title: full title linked to arXiv or official publication page.
- Method Name: short method/model name.
- Date: `YYYY/MM`.
- Domain/Task: manipulation, locomotion, navigation, offline RL, etc.
- Code: official repository if available, otherwise `-`.
- Venue: conference/journal name and year, otherwise `arXiv YYYY`.

## Placement Guidelines

- Add the paper to all clearly relevant sections (method and task views).
- Keep entries in reverse chronological order within each section.
- Avoid duplicates unless a cross-listing is genuinely useful.

## What We Accept

- Papers on action chunking, temporal abstraction, options, macro-actions, latent plans, and multi-step action prediction for control.
- Relevant robotics, RL, imitation learning, and offline RL works with clear chunking behavior.
- Surveys and benchmark papers directly tied to this topic.

## What We Do Not Accept

- Unrelated generic RL/control papers without chunking or temporal abstraction.
- Blog-only links or non-verifiable claims.
- Duplicate, promotional, or fabricated entries.

## Fixing Errors

If you find incorrect metadata or broken links:

1. Open an Issue with the problem.
2. Or submit a Pull Request with the fix.

## Questions

If unsure whether a paper fits, open an Issue first with paper link and short rationale.
