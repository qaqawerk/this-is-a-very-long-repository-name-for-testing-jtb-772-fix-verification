# Long Repo Name Test — JTB-772

Test repository created specifically to verify the fix for **JTB-772**
(`DataError: value too long for type character varying(64)`).

## Purpose

The repository name intentionally exceeds 64 characters (GitHub allows up to 100),
to confirm MyRepoBot correctly stores subscriptions/connections for such repos
after the storage field was widened from 64 to 255 characters.

## Usage

1. Push this project to GitHub under this exact repo name.
2. Connect MyRepoBot via `/connect`.
3. `/watch` this repository.
4. Trigger the daily connection refresh (or wait for it).
5. Confirm no crash and notifications work normally.
