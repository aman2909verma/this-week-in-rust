Title: This Week in Rust 328
Number: 328
Date: 2020-03-03
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/cmr/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

# Updates from Rust Community

## News & Blog Posts

[Rust in Blockchain Newsletter #9: The Month of Working from Home](https://rustinblockchain.org/2020/03/04/rib-newsletter-9-the-month-of-working-from-home/)
[The RustConf 2020 CFP is now open!](https://cfp.rustconf.com/events/rustconf-2020) We'd love to hear from you at RustConf!
- [Porting a JavaScript App to WebAssembly with Rust (Part 3)](https://www.slowtec.de/posts/2020-02-28-porting-javascript-to-rust-part-3.html)

# Crate of the Week

This week's crates is [tokenizers](https://github.com/huggingface/tokenizers), a Rust crate with python & nodejs bindings for fast text tokenization for machine learning.

llogiq (who singlehandedly selected the crate) is pretty self-congratulatory.

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [good first issue] [sqlx: Implement support for time-rs 0.2](https://github.com/launchbadge/sqlx/issues/115).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

304 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2020-02-24..2020-03-02

* [implement Associated Type Defaults](https://github.com/rust-lang/rust/pull/61812) (RFC #[2532](https://rust-lang.github.io/rfcs/2532-associated-type-defaults.html))
* [don't `bug` when taking discriminant of generator during dataflow](https://github.com/rust-lang/rust/pull/69562)
* [perf: buffer stderr when writing json errors/warnings](https://github.com/rust-lang/rust/pull/69227)
* [mark attributes consumed by `check_mod_attrs` as normal](https://github.com/rust-lang/rust/pull/69412)
* [stash API: remove panic to fix ICE](https://github.com/rust-lang/rust/pull/69623)
* [chalk: changes needed to build in rustc](https://github.com/rust-lang/chalk/pull/332)
* [adjust Miri value visitor, and doc-comment layout components](https://github.com/rust-lang/rust/pull/69257)
* [miri: let machine canonicalize AllocIDs](https://github.com/rust-lang/rust/pull/69408)
* [fail on multiple declarations of `main`](https://github.com/rust-lang/rust/pull/69379)
* [don't instantiate so many copies of `drop_in_place`](https://github.com/rust-lang/rust/pull/67332)
* [mark other variants as uninitialized after switch on discriminant](https://github.com/rust-lang/rust/pull/68528)
* [skip `Drop` terminators for enum variants without drop glue](https://github.com/rust-lang/rust/pull/68943)
* [audit liballoc for leaks in `Drop` impls when user destructor panics](https://github.com/rust-lang/rust/pull/67290)
* [add primitive module to libcore](https://github.com/rust-lang/rust/pull/67637)
* [relax str::get_unchecked precondition to permit empty slicing](https://github.com/rust-lang/rust/pull/69385)
* [fix aliasing violation in `align_to_mut`](https://github.com/rust-lang/rust/pull/69581)
* [add methods to 'leak' RefCell borrows as references with the lifetime of the original reference](https://github.com/rust-lang/rust/pull/68712)
* [stabilize `boxed_slice_try_from`](https://github.com/rust-lang/rust/pull/69538)
* [`BTreeMap` navigation done safer & faster](https://github.com/rust-lang/rust/pull/68827)
* [constify mem::forget](https://github.com/rust-lang/rust/pull/69617)
* [crates.io: enable sorting crates by most recently added](https://github.com/rust-lang/crates.io/pull/2214)
* [rustlings: add clippy lints](https://github.com/rust-lang/rustlings/pull/269)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [disposition: merge] [Cargo report future-incompat](https://github.com/rust-lang/rfcs/pull/2834).

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Permit negative impls for non-auto traits](https://github.com/rust-lang/rust/pull/68004).
* [disposition: merge] [Stabilize const for integer {to,from}_{be,le,ne}_bytes methods](https://github.com/rust-lang/rust/pull/69373).

## New RFCs

*No new RFCs were proposed this week.*

# Upcoming Events

### Africa

* [Mar  4. Johannesburg, ZA - Johannesburg Rust Meetup - Coffee and a chat about Rust](https://www.meetup.com/Johannesburg-Rust-Meetup/events/268960482/).

### Asia Pacific

* [Mar  5. Melbourne, AU - Rust Melbourne - Hack Night, Talks, and Networking](https://www.meetup.com/Rust-Melbourne/events/268002615/).

### Europe

* [Mar  4. Dublin, IE - Rust Dublin - Reboot pub meetup: The Duke](https://www.meetup.com/Rust-Dublin/events/237883717/).
* [Mar  4. Berlin, DE - OpenTechSchool Berlin - Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/gztznrybcfbgb/).
* [Mar  9. Karlsruhe, DE - Rust Meetup](https://www.meetup.com/Rust-Hack-Learn-Karlsruhe/events/268299172/)
* [Mar 11. Oslo, NO - Rust Oslo - Lightning talks](https://www.meetup.com/Rust-Oslo/events/268738879).
* [Mar 12. Turin, IT - Mozilla Torino - Gruppo di studio Rust alla Torino hacknight](https://www.meetup.com/Mozilla-Torino/events/268822794).

### North America

* [Mar  4. Indianapolis, IN, US - Indy.rs](https://www.meetup.com/indyrs/events/mffbtpybcfbgb/).
* [Mar 10. Denver, CO, US - Rust Boulder/Denver - March Meetup](https://www.meetup.com/Rust-Boulder-Denver/events/267834799/).
* [Mar 10. Redmond, WA, US - Seattle Rust Meetup - Monthly meetup in Redmond](https://www.meetup.com/Seattle-Rust-Meetup/events/prbtdrybcfbnb/).
* [Mar 11. Atlanta, GA, US - Rust Atlanta - Grab a beer with fellow Rustaceans](https://www.meetup.com/Rust-ATL/events/qxqdgrybcfbpb/).
* [Mar 11. Houston, TX, US - Houston Linux Users Group - Rust Study Group](https://www.facebook.com/events/469382520642102).
* [Mar 12. Columbus, OH, US - Columbus Rust Society - Monthly Meeting](https://www.meetup.com/columbus-rs/events/dpkhgrybcfbqb/).
* [Mar 12. Lehi, UT, US - Utah Rust - The Blue Pill: Rust on Microcontrollers](https://www.meetup.com/utah-rust/events/268567961/).
* [Mar 18. Vancouver, BC, CA - Vancouver Rust - Rust Study/Hack/Hang-out night](https://www.meetup.com/Vancouver-Rust/events/qnrgnrybcfbxb/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Infrastructure Engineer at Aleph Alpha, Heidelberg, Germany](https://aleph-alpha.de/sw_engineer.html?language=de).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Hi, fellow Crustaceans!
> I am a newbie of Rust programming language. A nauplius.

– [GhostProc on rust-users](https://users.rust-lang.org/t/how-can-i-improve-this/38711)

Thanks to [Tom Phinney](https://users.rust-lang.org/t/twir-quote-of-the-week/328/822) for the suggestions!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42) and [llogiq](https://github.com/llogiq).*

<small>[Discuss on r/rust]().</small>