# Full Validation Process #

## Starting the Build ##

1. Start up your VM.
2. refresh your VM.
3. `cd /vagrant/YOURREPO` (note that YOURREPO will vary depending on the name of your repository).
4. `git pull` your repository.
5. Run the command `sh scripts/validate.sh FOLIOURN`. `FOLIOURN` will be the full URN for the folio as an object (e.g. `urn:cite:hmt:msA.12r`)

Alternatively you can copy the script from your repository and paste it in the `scripts` folder in your shared repository. If you have more than one editing repository in your VM, it is recommended you rename it something obvious. You can then just run that file name in the terminal from anywhere.

## Handling the Results ##

1. The first file you will check is `hmt-mom/build/dse-validation-FOLIO.html`. FOLIO will correspond to the folio you checked. First check that all tests passed on this screen. If it is green then it means that the validator found text passages corresponding to all your indexed images. If it is not green, there should be a list of missed passages.
2. Then click the link for `inventory of FOLIO`, in the column `See Visual Inventory`. The FOLIO will correspond to the folio you checked. 
3. Review the image overlays for any obvious missing text passages. Adjust as necessary. Do not move on until you have passed this stage.
4. The second file you will check is `hmt-mom/build/hmt-validation-FOLIO/FOLIO.html`. FOLIO will correspond to the folio you checked.
5. There are four categories the validator checks: ethnic names, lexical tokens, personal names, and place names. There are three numbers that appear next to each one: number passed, number failed, and total.
6. Ethnic names, personal names, and place names will return errors if there is not a valid URN. There are several reason the URN might be invalid:
  1. you used a rejected URN, check the authority list to see if that item is supposed to be tagged and if there is a redirect
  2. mispelled URN, check your edition for proper spelling
  3. URN does not exist, you made up a URN that is not in the authority list yet. Be sure to request new personal and place names.
7. We also check ethnic, personal, and place names to make sure we are using the correct URNs, proofread even the ones that have passed because that test only checks whether it is a valid URN, not the correct one.
8. Lexical tokens will return errors for the following reasons:
  1. you made a mistake. Check your folio and the edition and fix.
  2. the scribe made a mistake (i.e. misspellings, extra accents/breathings or wrong accents/breathings). Check your folio and wrap the failure in `sic`.
  3. the scribe used a valid Byzantine orthographic equivalent (i.e. missed a breathing, accent, or iota subscript). Check your folio and submit an issue to [byzortho](https://github.com/homermultitext/byzortho/issues).
  4. the parser doesn't like it, but it's a valid word (capitalized words we don't tag, compounds that didn't resolve in morpheus; good rule of thumb is, if you can find it in the LSJ but it fails, it goes here). Check your folio and make an issue in [lexmapping](https://github.com/homermultitext/lexmapping).
  5. You missed a proper name that needs tagging.
9. When you've resolved all the failures, re-run the validator. Do not move on until your page passes at 100%.
10. When your page does pass at 100%. Submit an issue to [hmt-archive](https://github.com/homermultitext/hmt-archive/issues). Your issue should include the folio urn in the title and the version of validation in the text.
