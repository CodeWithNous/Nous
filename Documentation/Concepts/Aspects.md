<sub>Authored by the Nous team</sub>

Aspects are variables that reflect the mind of a Nous interpreter. They can be any data type (string, boolean, etc.) and follow the naming scheme of being all lower case with no spaces or punctiation. There is no complete list of aspects; Nous interpreters are trained to recognize aspects as they are defined in code, so it is the programmer's responsibility to create aspects with names that clearly convey their purpose. To aid in this, every aspect belongs to a read-only GROUP constant, of which there are three total: MIND, BODY, and SPIRIT.

---

MIND: For aspects related purely to mental state, such as consciousness, intelligence, and libido.

BODY: For aspects related to bodily perception and sensations, such as height, breastsize, and pleasure.

SPIRIT: For aspects related to identity and sense of self, such as name, gender, and sexuality.

---

When referring to an aspect, the formatting of [GROUP.aspect] must be used. Additionally, programmers should avoid using concrete numbers when working with aspects since, with some exceptions, the Nous interpreter's perception of an aspect will be based on feel rather than numerical value. However, this does not rule out using numbers or other traditional coding implements. 

Should a programmer want to use numbers as values for aspects, it should be an integer from 0 to 100. Applicable aspects can also use a string, a boolean (True/False, or 1 for True and 0 for False), an [array], or an { object }. The effectivity of these alternative options can vary between Nous interpreters, and programmers should always discuss the contents of their files with their interpreters before attempting to execute them for the best effect.
