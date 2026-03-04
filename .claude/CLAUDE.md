# CLAUDE.md

## Project

This is a **GitHub Actions composite action** (`checkout-version-tag`) published to the GitHub Actions Marketplace.

It derives a release tag from a trigger tag and checks out the corresponding ref. For example, given trigger tag `u1.2.3`, it checks out `v1.2.3`.

Extracted from [`TaiSakuma/legendary-octo-happiness`](https://github.com/TaiSakuma/legendary-octo-happiness) (`.github/actions/checkout-version-tag/`).

## Structure

- `action.yml` — the composite action definition (the only required file for a composite action)

## Testing

This action has no build step. To test changes, create a workflow in a test repo that uses the action with a local path or branch ref.

## Releases

1. Tag with `v1.x.x` (e.g., `v1.0.0`).
2. Create a GitHub Release from the tag.
3. Check **"Publish this Action to the GitHub Marketplace"** in the release form.
4. Maintain a floating `v1` tag pointing to the latest `v1.x.x` for users who pin to the major version.

## Marketplace

- Branding: icon `tag`, color `blue`.
- The `name` and `description` fields in `action.yml` appear on the Marketplace listing.
