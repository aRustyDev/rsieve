# Thoughts

## Email Server Functions

https://dev.to/biswasprasana001/building-an-email-server-components-and-how-they-interact-5fg8  
https://mailserverguru.com/email-server/  
https://www.xmox.nl  

- Model Ingestion
- MCP
- Envelope Encryption
- Opportunistic Encryption
- Post Quantum Encryption
- Tx Mail
- Shared Mailboxes
- Individual Mailboxes
- Selectable Identities
- Native Mail Relay Support
- Conversational Email (chat like)
- Channels/Feeds Concept
- Threads Concept
- Folders Concept
- Schedule Emails
- Keyboard Shortcuts
- Private instant reply (AI based SLM)
- Plugin/Extension First Architecture
  - grammarly
  - read response/email opened tracking
  - team/org only Commenting & tagging (internal)
  - CRM/CSM integrations
  - Calendar Integrations
  - Zoom/Video Conf Integrations
  - brand mgmt integrations
  - Tracker Stripping
- App Level Unsubscribe
- Sender Catalog (where did all emails uniquely get sent from?)
- Email Queueing
- Modes: Audience focused, Personal focused, CSM focused, Executive focused

## Sieve 2 functions

> Goals
> > Handle tagging & filing in a progressive manner
> > Put classes of emails in root dirs and then further move them down as rules narrow

- Flow Control
  - if, else, elsif, continue, stop, 
- Actions
  - reject, redirect, keep, discard, fileinto, expire, forward, tag
- Tests
  - address allof anyof envelope exists false header not size true
- Package Mgmt
  - require/import
- Lexical Tokens
  - comments testlist numbers string stringlist
- Variables
  - Variables, Const, Def
- Data Keys
  - body, header, tags, address, envelope, signature

```rust

const myList = ["a", "b", "c"];

fn doSomething() {
  fileinto "abc"
}

if (test) {
  let bar = foo();
} elif (test2) {
  let foo = bar();
}

match header.from {
  "a":
    doSomething();
  "b":
    doSomethingElse();
  _:
    stop
}
```
