# JSON transcriptions of supreme court cases
The included case details and justice details were mostly compiled from oyez and wikipedia. Some corrections were made by hand.

Also included for some cases are Wikipedia Infobox data. This information was only available for 1572 out of the 7687 total cases.

The case files are saved in JSON in the form:
```javascript
// ~/Downloads/transcripts/2018/Younger_v._Harris.js
{
    term: "1970",
    caseName: "Younger v. Harris",
    caseLink: "https://www.oyez.org/cases/1970/2",
    caseTranscripts: [
        {
            // transcript used from Apple_v_Pepper for demo purposes
            transcriptTitle: "Oral Argument - November 26, 2018",
            transcriptLink: "https://apps.oyez.org/player/#/roberts10/oral_argument_audio/24778",
            transcript: [
                {
                    {
                        speakerName: "John G. Roberts, Jr.",
                        textObjs: [
                            {
                                text: "We'll hear argument first ...",
                                start: 0,
                                stop: 6.56,
                                duration: 6.56
                            }
                        ]
                    },
                    {
                        speakerName: "Daniel M. Wall",
                        textObjs:[
                            {
                                text: "Thank you, Mr. Chief Justice, ...",
                                start: 6.56,
                                stop: 46.8,
                                duration: 40.24
                            },
                            {
                                text: "Sample text ...",
                                start: 46.8,
                                stop: 56.8,
                                duration: 10.00
                            }
                        ]
                    }
                }
            ]
        }
    ],
    decidedBy: "Burger Court",
    arguedOn: "Apr 1, 1969",
    petitioner: "",
    respondent: "",
    docket: "2",
    citation: "401\u00a0US\u00a037\u00a0(1971)",
    justiaLink: "https://supreme.justia.com/cases/federal/us/401/37",
    lowerCourt: "Federal district court",
    grantedOn: "",
    decidedOn: "Feb 23, 1971",
    wikiData: {
        title: "Younger v. Harris",
        Litigants: "Younger v. Harris",
        ArgueDate: "April 1",
        ArgueYear: "1969",
        ReargueDate: "April 29",
        ReargueYear: "1970",
        ReargueDate2: "November 16",
        ReargueYear2: "1970",
        DecideDate: "February 23",
        DecideYear: "1971",
        FullName: "Evelle J. Younger, District Attorney of Los Angeles County v. John Harris, Jr., Jim Dan, iane Hirsch, and Farrel Broslawsky",
        USVol: "401",
        USPage: "37",
        ParallelCitations: "91 S. Ct. 746; 27 [[L. Ed. 2d]] 669; 1971 [[U.S. LEXIS]] 136",
        Prior: "Judgment for plaintiffs, 281 [[F. Supp.]] [https://law.justia.com/cases/federal/district-courts/FSupp/281/507/1575355/ 507] ([[United States District Court for the Central District of California|C.D. Cal.]] 1968)",
        Subsequent: "",
        Holding: "The possible unconstitutionality of a state statute is not grounds for a federal court to enjoin state court criminal proceedings brought pursuant to that statute.  District Court for the Central District of California reversed and remanded.",
        SCOTUS: "1970-1971",
        Majority: "Black",
        JoinMajority: "Burger, Harlan, Stewart, Blackmun",
        Concurrence: "Stewart",
        JoinConcurrence: "Harlan",
        Concurrence2: "Brennan",
        JoinConcurrence2: "White, Marshall",
        Dissent: "Douglas",
        LawsApplied: "{{UnitedStatesCode|28|2283}}"
    }
}
```

An array of `caseTranscripts` is used to allow for cases that have more than one transcript as is the case with cases that lasted multiple days. `textObjs` is an array to allow for responses by individual speakers that are separated into separate paragraphs. As would be the case with:
> Daniel M. Wall
>
> Thank you, Mr. Chief Justice, and may it please the Court: The only damages theory in this monopolization action is rooted in a 30 percent commission that Apple charges app developers and which allegedly causes those developers to increase app prices to consumers.
>
> The case is barred by the Court's Illinois Brick doctrine because the developers' pricing decisions are necessarily in the causal chain that links the commission to any consumer damages. If the commission increases beyond the competitive level, but apps developers do not change their apps prices, consumers suffer no damages.


## Notes for Presidential party labelling in justices.js
------
John Marshall Harlan, Morrison Waite, Ward Hunt, William Strong, David Davis, Samuel Freeman Miller, Noah Hayes Swayne, Levi Woodbury, John McKinley, Philip Pendleton Barbour, Roger Taney, Henry Baldwin switched parties multiple times, but he switched for a last time before starting to serve as justice. There is no switch date marked.

Salmon P. Chase switched multiple times prior to serving as a justice, but only his switch during service is noted.

David Davis changed parties twice while serving as justice and once prior. His switch from Republican (1854-1870) to Liberal Republican (1870-1862) to Independent (1872-1886) is marked as a switch from Republican to Independent in 1870.

John McLean changed parties multiple times while serving as justice. Only his first and last party are noted.

No political party for William Cushing
