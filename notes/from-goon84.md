# re: the "impossible" release

I keep saying this in standup and everyone mutes me.

Previous release of this service **should not have been able to take the
Funhouse corridor offline** just because a desk password had special characters
in it. Special characters. In a password. That somehow queued enough reload storms
to look like an overload. That is not a normal failure mode. That makes no sense.
I have re-read the admission logs three times. Still nonsense.

We fixed the channel. We tightened the password box. We did **not** write a
real postmortem. See `notes/DRAFT-incident-blur.md` and then pretend you didn't.

- Goon84
