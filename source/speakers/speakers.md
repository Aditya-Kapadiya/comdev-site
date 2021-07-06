---
title: Listing yourself as a Potential Speaker
---

If you're an Apache committer, and you're interested in speaking about Apache 
Technologies, Apache Projects or the Apache Software Foundation as a whole, 
we'd encourage you to get involved and list yourself in our speaker 
application!

## Finding Speakers

If you are organising an event and looking for speakers, please see
[the Apache Speakers homepage](/speakers/) for details.

## Listing yourself as a Potential Speaker

To list yourself as someone interested in being an Apache Speaker, there are
two steps involved. The first is to create a FOAF file for yourself, including
a couple of key pieces of information. The second is to list yourself in the
speaking DOAP file.

### Creating your FOAF file

Creating a FOAF file for yourself is very easy, assuming you don't already 
have one available. Details on how to create a FOAF file, along with a
handy wizard to guide you through the process, are available at
[https://people.apache.org/foaf/](https://people.apache.org/foaf/) .

When creating your FOAF file, as a potential speaker we do require you
to include a few key bits of information. These are:

 * Your location
 * The projects you are involved in (include foundation wide ones too if you're
   happy to talk about these)
 * Your twitter ID (so we can point people at your speaking history on 
   [Lanyrd](http://lanyrd.com/))


### Listing yourself in the Speakers DOAP file

Now, if you haven't already done so, checkout the committers directory from
svn:

```
svn co https://svn.apache.org/repos/private/committers/
```

Edit *local-outreach/ApacheSpeakers.rdf* and add yourself in as a
helper. If your FOAF file is in svn and showing up on people.apache.org,
add in:

```
<helper>
  <foaf:Person rdf:resource="urn:org:apache:[your username].rdf" />
</helper>
```

If you have your FOAF file externally hosted, then the **rdf:resource**
should point to the URL of the file.

For an apache committer with username "foo", your entry would be one of:

```
<helper>
   <foaf:Person rdf:resource="urn:org:apache:foo.rdf" />
</helper>
<helper>
   <foaf:Person rdf:resource="https://www.example.com/foaf/foo.rdf" />
</helper>


Within 24 hours of committing your addition to
*local-outreach/ApacheSpeakers.rdf*, you should appear in the web
application as a potential speaker! Head over to 
[https://community.zones.apache.org/](https://community.zones.apache.org/)
a day later and check you're listed properly.
