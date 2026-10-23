# MomoMovies

A curator-led movie discovery app that helps you find the right film, 
matching what you're up for with what is available to watch.

**Explore MomoMovies: [momomovies.app](https://momomovies.app)**

<img width="898" height="750" alt="Momo Movies Discover page, Involvement set to Engaging or Intense with the Film Snob reputation filter active" src="https://github.com/user-attachments/assets/85369554-721e-4427-a57b-84b1f0ed7cef" />

*Start with the kind of viewing experience you want right now.*

## The idea

Finding a good movie is not the same as finding the right movie to
watch tonight.

MomoMovies starts with the viewer's current circumstances: how
demanding an experience they want, what kinds of films they are
interested in, and what they can actually watch. It uses those signals
to narrow a curated catalog into a more manageable set of choices.

The goal is not simply to recommend good movies. It is to help people
choose something that fits the moment.

## What it does

- **Involvement:** Choose how demanding an experience you want:
  Light, Engaging, or Intense. Films are matched on a calibrated
  intensity scale that considers emotional, intellectual, and sensory
  demands, not just genre or runtime.
- **Reputation:** Explore audience reception, awards recognition, and
  notable classics as separate signals rather than one blended score.
- **Streaming availability:** Titles show where they can be watched,
  based on the latest provider availability data MomoMovies has on
  record.
- **Personal context:** For signed-in viewers, recommendations can take
  account of movies they have watched, saved, or rated.

## How it works

- **Catalog:** Film records begin with TMDB data and are enriched with
  curated signals for audience reception, awards, and classics.
- **Availability:** MomoMovies uses provider availability data to help
  prioritize titles that are practical to watch. A planned
  reconciliation layer will add Watchmode links, pricing, and
  independent availability evidence while retaining conflicting claims
  for review rather than silently selecting a winner.
- **Personal matching:** The app is designed to work with incomplete
  viewing history without treating missing information as proof that a
  movie was never watched.
- **Viewing intensity:** Films receive a 1.0 to 3.0 involvement score
  through a combination of manual curation and calibrated estimates.
  Those scores power the Involvement filter.

## Design challenges

1. **Availability changes constantly.** Provider catalogs churn,
   editions differ, and regional windows shift. MomoMovies treats
   availability as evidence with freshness and provenance, rather than
   a permanent property of a title.

2. **Viewing histories are incomplete.** A lifetime of movie watching
   is often recorded unevenly. The app needs to be useful without
   inventing certainty about what someone has seen or how they felt
   about it.

3. **Recommendations should be explainable.** Curated scores and
   calibration versions are preserved so the app's behavior can be
   understood, reviewed, and improved over time.

## Screenshots


<img width="933" height="729" alt="Momo Movies Discover page with the Safe Bet preset selected and a title preview open, showing awards recognition, audience reception, streaming availability, and the Hide, rate, and Stash actions" src="https://github.com/user-attachments/assets/1f4c120b-911e-4404-885f-84380967b823" />

*Same page, different quickset: Safe Bet this time, with a title preview open. The preview shows recognition, reception, availability, and when signed in adds the quick actions Hide, rate, and Stash.*

<img width="934" height="730" alt="Momo Movies results grid: film cards with poster, title, director, lead actors, year, and runtime, narrowed by the active filters shown at the bottom — Contemporary, under 2 hours 10 minutes, free to watch, unanimous praise, Light or Engaging." src="https://github.com/user-attachments/assets/cc192b93-9bd3-41e1-8027-afa29fee14a4" />

*Explore the resulting selection of films, with options to sort, change the display, or narrow it to the Highlights.* 

## Status

MomoMovies is live and in active development. Designed by Moshe Kahn
and built with an AI-assisted development workflow using Codex.

Development history: [CHANGELOG.md](CHANGELOG.md)

The source code remains private while the app is being built; this
repository is its public showcase. MomoMovies is part of
[The Moments Collection](https://kahntra.com/), a body of
context-aware tools for everyday decisions.

Built with Svelte, TypeScript, Vite, and Supabase.
