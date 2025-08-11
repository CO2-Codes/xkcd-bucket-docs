# Important note

Bucket's documentation was moved here from the previous location after some discussion with the #xkcd ops in August of 2025, because of technical problems with the old location.
However, it was moved as-is and CO2 found several pieces of documentation to be _outdated_.
We could use your help updating this documentation. You don't need to be knowledgeable about Github - if you're not sure where to start just talk to CO2 on IRC.

[You can find a list of unfinished tasks here.](https://github.com/CO2-Codes/xkcd-bucket-docs/blob/main/META.md#todo)

----

----

----

Bucket has an outer shell of metal;<sup>[_citation needed_]</sup> within the metal is a protective layer of high density plastic,<sup>[_citation needed_]</sup> in which may or may not reside pure HOH.<sup>[_citation needed_]</sup> There<sup>[_citation needed_]</sup> can only be speculation about what else the Bucket contains.<sup>[''citation needed'']</sup>

# Using the #XKCD Bucket
1. Do not make our Bucket stupid or mean. Any stupiding of the Bucket may cause an op to tell Bucket to ignore you.
2. Bucket's replies should generally not be meaner or more asshole-y than the lines that trigger them.
3. <del>Do not alter factoids that are not your own. </del> Nobody owns any factoids.
4. Only the ops are allowed to cull stupid or useless factoids. And they will, boy howdy they will. The only exception to this rule is if the factoid is about you -- if someone writes an abusive factoid about you and the ops have not corrected it, please feel free to edit it yourself.
5. Using Bucket as a surrogate asshole will result in either a revocation of your Bucket privileges or having your ass kicked from here to Pakistan (unless you live in Pakistan, in which case you will be booted to occupied North Texas). **Making abusive, mean factoids about anyone else is strictly outlawed** and if you are caught doing it, you will be harshly dealt with. Please tattle on anyone you see adding abusive factoids, whether in #xkcd or #bucket.
6. Do not attempt to have Bucket trigger another #xkcd bot.  It won't work, don't try, you'll just really annoy those who have to clean up your mess.  Do it enough and actions will be taken to correct the situation.
7. Do not try to put a variable in a factoid trigger. It does not work that way.

# Addressing
You need to address Bucket directly to teach him factoids; you can do so by prefixing your message "Bucket," or "Bucket:" (Your IRC client may automatically do this).

## If Bucket doesn't reply
- Make sure you're prefixing messages properly. "Bucket~ [command]" and "Bucket   [command]" will not trigger him.
- Bucket will not trigger non-addressed factoids which are shorter than 6 letters long. "Bucket, dogs" will trigger bucket. "Dogs" on its own line will not. "Bucket, how2love" and "how2love" will trigger the same factoid.
- In PM, do not preface your commands with "Bucket, ", just use the [command] directly. You can only query, you cannot teach factoids in PM.
- Bucket might be shut up at the time. Use #bucket or PM to check.
- Bucket might be ignoring you -- and only you -- because an op has told it to. Probably because you put in some bad factoids.

# Teaching factoids to Bucket
#### X is Y
The most common type of factoid you can teach to Bucket is by simply saying "X is Y". If someone says "X" later on, Bucket will reply "X is Y"
- Be careful about accidentally creating a new factoid while talking to Bucket.
- You can also say "X is also Y", this was formerly required to attach multiple factoids to one trigger so you may see older users use this.
- If you type "X is Y is Z", Bucket will split it on the first "is", making the trigger "X" and the factoid "Y is Z" and Bucket will respond "X is Y is Z".  
- If you wanted 'X is Y' to trigger 'Z', teach Bucket 'X is Y \<is\> Z'.  See \<verb\> below.

### X are Y
Similar to "X is Y", you can teach this kind of factoid by simply saying "X are Y" and if someone says X later on, Bucket will reply "X are Y"

### X \<verb\> Y
You can use other things instead of "is" or "are" by putting them inside greater and lesser-than signs, such as "X \<hates\> Y" or "X \<compliments\> Y"

### X\<'s\> Y
After using this, if someone says "X", Bucket will respond "X's Y".
- Apostrophes - learn how to use them before using this.

### X \<reply\> Y
You can say "X \<reply\> Y", when someone says "X", Bucket will respond "Y".
- You might see some people using "X is \<reply\> Y", this was formerly required so you may see older users use it.

### X \<action\> Y
If you use "X \<action\> Y", when someone says "X", Bucket will use "/me Y".
- Like the above two types, retain the greater-than and lesser-than signs.

### Slash commands
Bucket is not run on a client; she is his own entity.  This means that slash commands (things like /me, /msg, /quit, etc) **do not work. Do not put them in**, you'll only anger those who have to clean up your mess.  
- Also, escaping (using the \ to get things like question marks to go in on a factoid) is no longer needed.

### Remember quote
If you type "remember {nick} {snippet}" where "{snippet}" is a snippet from a line that has been said by the person in "{nick}", Bucket will remember that factoid under the trigger "{nick} quotes". When that quote factoid is triggered, Bucket will respond "\<Example\> Lorem Ipsum"
- If you see a person known as "Spork" say something that you wish to quote with the "remember" command, '''don't do it.''' The fury of a thousand fish will descend upon you.
- When Bucket is remembering a "/me" action, instead of the regular "\<Example\> Lorem Ipsum" he'll say "* Example lorem ipsumed."

## Searching for factoids
### Listing factoids
"literal X" will give you a list of factoids associated with that trigger separated with "|". If the list of factoids is too large, Bucket will put them them on another "page" and indicate how many factoids are on the subsequent pages by appending something like "72 more" on the list of factoids. You can browse the next pages by using "literal\[2\] X", replacing "2" with the number of the page you wish to check.

### List factoids in a text file
Typing "literal\[*\] X" will make Bucket produce a url linking to a text file of all the factoids associated with that trigger.

### Triggering a specific factoid
"X =~ /m/" will make Bucket reply with the first factoid in that trigger which contains "m".

### Listing the details of a factoid
"what was that?" will make Bucket list the factoid's details thusly: "That was X(#77777): \<reply\> Y", the number being the factoid's ID.

## Editing factoids

### Substitution editing
Telling Bucket "X =~ s/m/n/" will replace "m" with "n" in the factoids for the trigger "X". Adding an "i" flag ("X =~ s/m/n/i") replaces case-insensitively. If there are multiple occurrences of "m", Bucket will edit the first instance in the trigger's first matching factoid. Ops can add a "g" flag to replace all occurrences.

Slashes should not be backslash-escaped in the string--use any other delimiter, such as a comma, as a replacement for slashes. Example: to change "`The best site \<is\> http://google.com/search`" to "`The best site \<is\> http://xkcd.com`", you could type: "`Bucket: The best site =~ s,http://google.com/search,http://xkcd.com,`"

### Undo
"undo last" undoes the last change made to a factoid (editing one, adding one, deleting one.)  Non-ops can undo last only if they made the last change.

## Word class variable
Putting a word class variable in a factoid will replace the variable with a word from the appropriate word class. Variables apply only to Bucket's responses. For example, telling bucket "play with $who \<reply\> what would you like me to play with $who?" will not work.

### $noun
Use "$noun" to place a noun variable which will become a noun when the factoid is triggered.
- Bucket will properly work when you use "a $noun" and "$nouns"

### $verb
Use "$verb" to place a verb variable which will become a verb when the factoid is triggered.
- Bucket will also properly work with "$verbs", "$verbed" and "$verbing"

### $adjective
Use "$adjective" to place an adjective variable which will become an adjective when the factoid is triggered.

### $preposition
Use "$preposition" to place a proposition variable which will become a preposition when the factoid is triggered.

## Username variables
Putting a username variable in a factoid will replace the variable with a username when triggered.

### $who
"$who" will be replaced by the name of the person who triggered the factoid.

### $someone
"$someone" will be replaced by a username chosen from recent posters.
- "$someone" used to be completely random, but was changed so that Bucket doesn't bother idle users as much.

### $to
"$to" will be replaced by the intended recipient, e.g. "\<Someone\> Bucket: yada yada" will replace $to with Bucket. If there is no intended recipient, it will fall back on $someone.

### $op
"$op" will be replaced by the name of one of the Ops. **WARNING:** This might get you kicked/banned!

## Object variables

### $vehicle
"$vehicle" will be replaced with a vehicle.

### $room
"$room" will be replaced with a room.

### $ejaculation
"$ejaculation" will be replaced with a exclamation. _Support for this feature is deprecated_

### $celebrity
"$celebrity" will be replaced with a name of a celebrity.

### $mood
"$mood" will be replaced with a name of a mood.

### $color
"$color" will be replaced with the name of a color.

### $bodypart
"$bodypart" will be replaced with a (probably not scientific) name of a body part.

## Number variables

### $digit
"$digit" will be replaced with a random digit from 0 to 9.

"$nonzero" will be replaced with a random digit from 1 to 9.

## Inventory
Bucket uses the new RFC inventory system. A general ideas-ish page is at [Bucket_inventory]. **(CO2 note: TODO: fix link or remove it)**

### Listing Bucket's inventory
Address "inventory" to Bucket to get a list of what Bucket contains.

### Adding new items to inventory
You can give Bucket new items by making a message that follows the basic patterns outlined below. (Replacing {item} with the object you wish to give to Bucket.)
- \* Randall puts {item} in Bucket.
- \* Randall gives Bucket {item}
- \* Randall gives {item} to Bucket

.
- Bucket will ignore your attempt to keep an item in him if the line ends with a question mark.
- Bucket will also ignore your attempt to keep an item in him if the message contains the word "to".

Bucket will replace the word "his" or "her" with  "{nick}'s", with {nick} being the nick of the person giving him the item. Example: "Randall gives Bucket his banana" would add "Randall's banana" to Bucket's inventory.
Bucket will not accept duplicate items.

### Deleting inventory items
Ops can delete items from the inventory (which will also stop them from ever being automatically created) using the 'detailed inventory' and 'delete item #X' commands.

### Inventory variables

#### $item
"$item" will be replaced by a randomly selected item from Bucket's inventory.

#### $giveitem
"$giveitem" will be replaced by a randomly selected item from Bucket's inventory and will discard the item.
- Use sparingly. Creating a factoid that discards many items will make a fury of ten thousand toilet rolls descend upon you.

#### $newitem
"$newitem" will be replaced by a randomly selected item from a list of various items Bucket has accumulated over time and will then add the item to his current inventory.

## Gender
Bucket now has support for genders with the RFC [Bucket_Gender]. **(CO2 note: TODO: fix link or remove it)**
More specifically, you will be able to tell Bucket by which pronoun you would like to be referred to.

### Grammatical genders

This is a table of the five types of genders that you can choose and what pronouns are associated with them:

| Grammatical Gender | Subjective |  Objective | Reflexive | Possessive Pronoun | Possessive Determiner |
| ------------------ | ---------- | ---------- | --------- | ------------------ | --------------------- |
| Male               | he         | him        | himself   | his                | his                   |
| Female             | she        | her        | herself   | hers               | her                   |
| Androgynous        | they       | them       | themself  | theirs             | their                 |
| Inanimate          | it         | it         | itself    | its                | its                   |
| Full name          | \<name\>   | \<name\>   | \<name\>  | \<name\>'s         | \<name\>'s            |

- The male set of pronouns uses the traditionally male pronouns, "he", "him" and "himself".
- The female set of pronouns uses the traditionally female pronouns, "she", "her" and "herself".
- The androgynous set of pronouns uses the gender neutral singular they, "they", "them" and "themself".
- The inanimate set of pronouns uses the gender neutral "it", often used on inanimate objects, "it" "its" and "itself".
- The Full name set of..."pronouns" simply uses the user's name.

### Setting and looking up genders
You can set your own gender by addressing "I am {gender}" to Bucket, replacing "{gender}" with the gender of your choice.

You can ask what is the gender of another user by asking "what gender is {username}"

### Gender Variables
The following variables can be used in factoids, and will use the correct pronoun if a factoid contains $someone or $who.

|              | Subjective | Objective | Reflexive | Possessive Pronoun | Possessive Determiner |
| ------------ | ---------- | --------- | --------- | ------------------ | --------------------- |
| **Variable** | $subjective, $shehe, $heshe, $he, $she, $they, $it | $objective, $him, $her, $them, $himher, $herhim| $reflexive, $himselfherself, $herselfhimself, $himself, $herself, $themself, $itself | $possessive, $hishers, $hershis, $hers, $theirs | $determiner, $hisher, $herhis, $their |

## Special Factoids
There are a few factoids that are used to generate replies to specific situations:

#### Don't know
Called when a factoid is requested that has no values. These responses are taught by the channel ops. (I don't know anything about that.)

#### Band name reply
Called randomly when someone uses a short phrase that sounds like a band name (\<reply\> "$band" would be a good name for a band.)

#### Tumblr name reply
Called randomly when someone uses a short phrase that sounds like a tumblr name (`<reply> http://$band.tumblr.com`).

Sometimes the tumblr name is so awesome that a [denizen] creates it. A list of Bucket-created tumblrs can be found [here]. **(CO2 note: TODO: fix links or remove it)**

#### Duplicate item
Called when someone puts an item that is already in the inventory (<\reply\> $who: I already have $item.)

#### Drops item
Called when an item drop is forced (\<action\> fumbles and drops $giveitem.)

#### Pickup full
Called when an item is handed to a user, but (s)he has already been given something (\<action\> hands $who $giveitem for $item)

#### Takes item
Called when an item is taken (\<action\> is now carrying $item.)

#### List items
Called when someone asks for Bucket's inventory (uses variable $inventory)

#### Uses reply
 Called when someone says "uses \<XYZ\>"

#### Automatic Haiku
:Called when a haiku is detected

## Special Functions (non-factoids)
#### 10+2
Bucket can do basic math (+,-,*,/,**). For that to work he needs to be addressed, the line may only contain numbers and the aforementioned operations and there must not be a factoid for it (as example, 1+1 has its own factoids).

#### bad-ass
If a message contains a phrase similar to $adjective-ass $noun (like bad-ass car), Bucket will shift the hyphen. See also [Hyphen](https://xkcd.com/37/)

#### Do you know?
If a message starts with the phrase "do you know", Bucket will respond with "No, but if you hum a few bars I can fake it.

#### Say it again
If anybody says a line that starts with "say" and Bucket is not being addressed, Bucket will repeat everything after say followed by an exclamation mark.

#### sexchange
If a message contains a word starting with ex, there's a random chance Bucket will repeat the phrase, substituting ex with sex

#### super effective!
If anybody says a line (or performs an action) that starts with "uses", Bucket may respond with "It's super effective!"

#### TLA
:A three letter acronym without any punctuation will cause Bucket to respond with a potential meaning of the three letter acronym, even when not addressed. The meanings are phrases Bucket considers good band names.

#### the fucking
:If a message contains the phrase "the fucking", Bucket will swap both words

## Twitter Bucket
A limited version of Bucket has [joined twitter](https://twitter.com/xkcdbucket) on May 6th, 2009. **(CO2 note: TODO: remove link to hellsite?)**

## Excellent Factoids
These factoids are pretty neat. If you want to trigger more than one, or see the full contents, please go to #bucket.

- "Newbie pack" should be triggered for oblivious or clueless lusers.
- "[Choose Your Own Misadventure]" is pretty epic. Ayup. **(CO2 note: TODO: fix link or remove it)**
- "What time is it?" should give some interesting results
- "Choose me a snack" is delicious botism
- "Choose me a drink" is effective
- "Choose me a beer" is a work in progress
- "Choose me a car" is a work in progress
- "Botsnack" may overexcite Bucket & co
- "Annoy {user}" can be entertaining, if {user} is somewhat well known (most ops)
- "Randall?" contains extensive documentation on the function and nuances of the author of this most illustrious wobcomec.
- "AWESOME" contains many things which may or may not be awesome.
- "Hack yourself" is a work in progress
- "find a random item" yields bizarre results
- Bucket can create "boss fight"s for you.
- 'relsqui' and 'Frowardd' have carefully curated factoids. Same for 'Spork quotes'.
- "Ruin a childrens book" will do what it says on the tin.
<!-- YOU WILL SERVE LORD DAGOTH, AS FLESH OR DUST!!!! -->

## Filling silence
If nobody has said anything in a while (about three minutes), Bucket will sometimes quote something from one of the following websites:

**(CO2 note: TODO: I think all of this is disabled, remove links?)**

- [MyLifeIsAverage](http://mylifeisaverage.com/)
- [Shit My Dad Says (Twitter)](http://twitter.com/Shitmydadsays)
- [Fake AP Stylebook (Twitter)](http://twitter.com/FakeAPStylebook)
- [Fake Animal Facts (Twitter)](http://twitter.com/FakeAnimalFacts)
- [God Damn Batman (Twitter)](http://twitter.com/God_Damn_Batman)

If Bucket doesn't quote one of the websites, he displays a random factoid.

## Variable editing
Some variables can be edited.

### Editable variables
- All editable variables are currently protected, which means they cannot be edited by normal users.

Parts of speech
- $adjective
- $adverb
- $article
- $noun
- $preposition
- $soiafpreposition
- $verb

People
- $band
- $op
- $celebrity

Places
- $country
- $room
- $state
- $place

Things
- $bodypart
- $color
- $ejaculation
- $gait
- $mood
- $occupation
- $profession
- $official
- $vehicle
- $weekday

Critters
- $animal
- $op
- $pokemon

Numbers
- $digit
- $nonzero
- $hex

### Listing
#### Listing editable variables
Address "list vars" to Bucket to get a list of known variables that are editable.

#### Listing the values in a variable
You can get all the values in a variable by using "list var {variable}" with "{variable}" being replaced by the variable you wish to see.
- Bucket will display a link to the list of variables if there are too many variables to list. (Similar to literal\[*\])

### Editing variables
#### Adding to a variable
Addressing "add value {variable} {value}" (replace "{variable}" with the variable you wish to add to and replace "{value}" with the thing you wish to add to the variable) to Bucket will add a value to that variable.

#### Removing from a variable
"remove value {variable} {value}" (again, replace "{variable}" with the variable you wish to remove from and replace "{value}" with the thing you wish to remove from the variable).
- Do this if you have a good reason for doing it.

#### Setting a variable type
"var {variable} type {var|verb|noun}" Sets the "type" of a variable.  Verb type variables can accept a "-ing" and "-ed" and "-s" suffix, while noun types can accept "-s" and update the "a/an" prefix. You can see whether a variable what type a variable is by using "list vars" and checking if there is a "(n)" for noun-types or a "(v)" for verb-types behind the variable.

## User Commands

#### Adding factoids
- X is Y
- X are Y (plural)
- X \<reply\> Y
- X \<action\> Y
- X \<verb\> Y
  - For example: X \<drinks\> Y
  - It lets you use a verb that isn't "is" or "are"! 

#### Bucket, literal X
- gives the first few factoids for X

#### Bucket, literal\[#\] X
- pages through the next factoids for X
 
#### Bucket, literal\[*\] X
- dump out all the factoids for X to a URL

#### List items
- Lists out the current inventory.

#### Bucket, X =~ /phrase/
- pick a factoid at random from the factoids of X that includes 'phrase'

#### Bucket, X =~ s/a/b/
- bucket will replace the first instance of "a" it finds with "b" in the factoid called X

#### Bucket, undo last
- undo the last modification made (only works if it was done by the same user who calls undo)

#### $who 
- when a factoid is triggered, all instances of this keyword will be substituted for by the nick of whomever triggers the factoid.

#### $someone
- replaces with the nick of a random person who may or may not be in channel at the time.

####  $item
- replaces with a random item in his inventory.

#### $giveitem
- replaces with a random item in his inventory, and deletes that item.

#### Bucket, shut up
- stop talking in channel for one minute.

#### Bucket, stats
- Give some numbers on what Bucket knows and has learned.  The totals update every 10 minutes or so.

#### Bucket, something random
- Show a random factoid.

#### Bucket, what was that?
- will respond with the factoid related to the last tidbit uttered.

#### Bucket, list vars
- show all the defined variables

#### Bucket, list var {variable} 
- show all the values of a variable (or at least as many as would fit in one line)

#### Bucket, add value {variable} {value}
- add a new value to the already defined variable (only if it's unprotected)

#### Bucket, remove value {var} {value}
- remove value <value> from variable (only if it's unprotected)

#### Bucket, remember {nick} {snippet}
- Look in the last few lines in channel for a line containing the partial line mentioned.  If found, add it to a 'nick quotes' factoid in the form of \<{nick}\> {line that was found}'.  The number of lines remembered per channel is controlled by the history_size parameter.

#### Bucket, I am {gender}
- Tell bucket what gender he should use to refer to you.  See the gender docs for complete details.

#### Bucket, what is my gender?
- Ask bucket to report your gender.

#### Bucket, restore topic
- Ask Bucket to restore the previous topic in the current channel, if possible.

#### Bucket, how many syllables in {word}?
- Find the number of syllables Bucket believes to be in the word, as used to find haiku.

### Ops only commands

#### Factoids

##### Bucket, alias X => Y
- make requests for X return Y.  Can be chained, cannot be looped.

##### Bucket, merge X => Y
- first move all of the existing factoids from X to Y.  Then create an alias.  Cannot (currently) be undone.

##### Bucket, delete X
- delete all the factoids for X.

##### Bucket, delete #nnnnn
- delete the factoid numbered #nnnnn.

##### Bucket, forget that
- delete the most recent factoid referenced in this channel (only that answer, not the entire factoid).

##### Bucket, forget #nnnnn
- delete the factoid numbered #nnnnn.
- this doesn't work in private messages unfortunately.

##### Bucket, undo last \[#channel\]
- undo the last change made in channel (or in the specified channel).

##### Bucket, protect X
- lock down all the factoids for X, so only ops can modify them.  If X is $var, will protect the variable so only ops can add values to and remove values from it.

##### Bucket, unprotect X
- opposite of protect.

##### Bucket, lookup #n
- Show the factoid with ID of n.

##### Bucket, load plugin foo
- Look for, and load the plugin named 'foo'. Should be found in the plugins directory, with the name plugin.foo.pl

##### Bucket, unload plugin foo
- Remove the previously loaded plugin

#### Variables

##### Bucket, create var {variable}
- creates a new variable with that name.  By default, new variables are always protected.

##### Bucket, remove var {variable}
- delete the variable.  

##### Bucket, protect X
- lock down all the factoids for X, so only ops can modify them.  If X is $var, will protect the variable so only ops can add values to and remove values from it.

##### Bucket, unprotect X
- opposite of protect.

#### Items

##### Bucket, delete item #X
- delete item #x from Bucket's carried inventory and from the database.  Use 'detailed inventory' to get the item numbers for the current inventory.

##### Bucket, detailed inventory
- list all the items currently carried with item numbers.  Required before a 'delete item #X' command can be used.

#### Settings

##### Bucket, set X Y
- Set variable X to Y.  If Y isn't specified, will list all valid configuration variable names.

##### Bucket, get X
- Read the value of X.

#### Users

##### Bucket, ignore X
- Ignore anything X says.

##### Bucket, unignore X
- Stop ignoring X.

##### Bucket, list ignored
- List all who are currently ignored.

##### Bucket, exclude X
- Don't consider X as a valid $someone.

##### Bucket, unexclude X
- Restore X to the possible list of $someone.

##### Bucket, {nick} is {gender}
- Set the gender for {nick}.  See gender docs for the complete details.

##### Bucket, don't quote {nick}
- Don't allow the 'remember' command to be used on <nick>.

##### Bucket, do quote {nick}
- Undo the 'don't quote' command.

#### Miscellaneous commands

##### Bucket, shut up|go away
- stop talking in channel.  Bucket will still respond to queries from ops.

##### Bucket, shut up for (a min|a moment|a bit|a while)
- shut up for some time then come back (60 sec|1 min ± 30 sec|6 min ± 2 min|45 min ± 15 min).  (Ops only; non-ops can say shut up for however long, but Bucket will still only leave for the usual amount of time)

##### Bucket, shut up for nnn(s|m|h)
- shut up for nnn seconds, minutes or hours, then come back.  (Ops only; non-ops can say shut up for however long, but Bucket will still only leave for the usual amount of time)

##### Bucket, unshut up|come back
- resume talking in channel.  (Ops only)

##### Bucket, join #X|part #X
- guess!

##### Bucket, stat keys
- List all the known statistic keys.

##### Bucket, stat {key}
- Get the value of that particular key.

##### Bucket, restore topic #channel
- Ask Bucket to restore the previous topic of #channel, if possible.

##### Bucket, {word} has {number} syllables
- Advise Bucket of the number of syllables in the word.
