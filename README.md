# Node Auth 1 Guided Project

Guided project for **Node Auth 1** Module.

## Prerequisites

- [SQLite Studio](https://sqlitestudio.pl/index.rvt?act=download) installed.

## Project Setup

- [ ] fork and clone this repository.
- [ ] **CD into the folder** where you cloned **your fork**.
- [ ] type `npm i` to download dependencies.
- [ ] type `npm run server` to start the API.

Please follow along as the instructor adds authentication to the API.

## Encryption vs Hashing

- for password storage, use hashing. (use hashing because encryption is two-way), but hashing is one way.  Once hashed, there is no (easy) way of getting the original  string back (passowrd).

## Auth workflow

- register an account.
- login.
- log out.
- restrict access to resources.

## Tokens
- the server does not store info, the info is stored on the token. There is nothing to destroy

## Server
- on successeful login/register, produce and send a token
- send token to the client
- on following requests, verify the token
- if token is good, provide access, if not block access.

## Client
- store the tooken (memory, local storage, header .....)
- send the token on every request
- destroy the token on logout