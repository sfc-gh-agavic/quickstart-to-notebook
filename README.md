# CURSOR CREATES A SINGLE NOTEBOOK FROM A QUICKSTART

This project demonstrates how to leverage Cursor AI to streamline the creation of Snowflake demos. You'll learn how to use AI assistance to consolidate quickstart materials into executable notebooks and customize advanced implementations efficiently.

This project uses the Dynamic Tables quickstart for it's context.

## EXAMPLE 1: USING CURSOR TO CONSOLIATE A QUICKSTART INTO A SINGLE NOTEBOOK

STEP 1 - Manually type out a very simple set of instructions.
In this case, we're asking to consolidate existing code in a quickstart into a single notebook.
See PROMPT1.md for those instructions and general format.

Note: There are many ways to create instructions, a PRD, etc.  This excercise is encouraging 
simplicity as only a single notebook is created.  See FAILED PROJECTS below for what can go 
wrong when the AI trying to do more than is actually required.

STEP 2 - Prompt Cursor to build the notebook
"Create the required notebook as outlined in @PROMPT1.md "
Note: You should just have the PROMPT1.md file as context (not this README.md too) 

STEP 3 - Click through all the Cursor messages (continueing after 25 calls, Keep All, etc)

STEP 4 - Import the notebook into Snowsight and update cell types as needed
Sometimes markdown and SQL cells will need flipped to their appropriate type

STEP 5 - Execute the notebook and complete the quickstart

STEP 6 - Export the final notebook to your project
eg: DYNAMIC_TABLES_QUICKSTART_VALIDATED.ipynb
Show it to your customer.  Or better, have them run it in a HOL!

## Files for Example 1
- PROMPT1.md
- dynamic_tables_demo.ipynb (just an example generated file)
- DYNAMIC_TABLES_DEMO_VALIDATED.ipynb (to be created by user)



## EXAMPLE 2: QUICKSTART CUSTOMIZATION

STEP A - Manually type out a very simple set of instructions.
In this example we want Cursor to help us further customize the quickstart. The details are in PROMPT2.md

STEP B - Prompt Cursor to build a file
"Create the list of query examples in a new file called QUERY_EXAMPLES.md as outlined in @PROMPT2.md "

STEP C - Review QUERY_EXAMPLES results
This is where you will likely experiment with the instructions you give.
If you don't like the QUERY_EXAMPLES doc, you could manual edit it directly 
  or modify PROMPT2, delete the QUERY_EXAMPLES doc, and go back to STEP B for recreation.

STEP D - Manually type out a new set of instructions.
In this example we want Cursor to incorportate some of the Query Examples it generated from Step B into the quickstart. The details are in PROMPT3.md

STEP E - Manually create a new notebook
Save a copy of DYNAMIC_TABLES_QUICKSTART_VALIDATED.ipynb as DYNAMIC_TABLES_ADVANCED.ipynb
We'll have Cursor modify this new file so we can retain the VALIDATED version for reference.

STEP F -  Prompt Cursor to modify the notebook with a smaller set of Query Examples.
"Execute @PROMPT3.md"

STEP G - Validate results
It should look good. :)

If there were any issues with the notebook changes, you again can choose to manual edit the result OR
further improve our understanding of prompt engineering with Cursor. This is done by modifing PROMPT3, 
deleting the ADVANCED notebook, and going back to Step E with a clean notebook.

At this point you could continue the prompt & build process to add the remaining query examples. Have fun!

## Files for Example 2
- PROMPT2.md
- PROMPT3.md
- QUERY_EXAMPLES
- DYNAMIC_TABLES_ADVANCED.ipynb  ( you be created by the user and modified by cursor)


## OTHER EXAMPLES - FAILED PROJECTS
You will see two directories in this project (FAIL1, FAIL2).

These are included to showcase how asking Cursor to perform tasks that are too open-ended or with too many details may result in a very complicated project.  Some projects may require complexity, but the general approach is still to guide the AI through detailed, validated, incremental steps.

- FAIL1 = Asking for a comprehensive Product Requirement Document (PRD) resulted in just that.  Way too much detail for this use case.
- FAIL2 = A simplified PRD was used to outline the project and create a notebook. It unfortuantely created a notebook for Cursos, not Snowsight.  We could have iterated off this solution, but decided to deviated to an even more simplistic, incremental creation process.