# Strandings911

this is the list of changes made by Dina Li and suggested follow-up tasks

for all of these, check that the list of locations is correct, I added the new locations AFTER the current locations

ARAMessageViewController -- added new locations

ARAGPS -- added new locations here: withinServiceArea(), inStateWatersAt()

isLocationOffshore(), TODO: do additional polygons need to be added here??

ARAQuestionViewController -- added new locations; TODO: consider replacing HTML with an external file for security reasons

Category.h and Category.m -- there seemed to be a problem with using the word "Category" - it's a reserved word, so I renamed the files NOAACategory.

ARAMammalPreload.m  -- create new species; I added the meta data information about the new species such as the Family; ToDO: add the descriptions, I didn't have all the details for the new ones

ARAReportViewController -- created a pList and added ALL the old and new locations. TODO: check for accuracy especially states such as Massachusetts which has three sub-areas - phone and state full name may be wrong. I don't know how the placemarks returns locations such as Massachusetts_Central? Is the "debug phone number" still necessary? I wasn't sure how to use it, so I included it in every state. It would be better to remove it so that the .pList is shorter.

