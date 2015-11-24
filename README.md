# Strandings911

this is the list of changes made by Dina Li and TODOs

for all of these, check that the list of locations is correct, I added the new locations AFTER the current locations

/* current version */ LOCATION IS HARD CODED to Connecticut

TESTING - I had trouble testing when I was in my office, it seemed to work better at home even when the location is hard coded. 

ARAMessageViewController -- added new locations

ARAGPS -- added new locations here: withinServiceArea(), inStateWatersAt()

isLocationOffshore(), TODO: do additional polygons need to be added here??

ARAQuestionViewController -- added new locations; TODO: consider replacing HTML with an external file for security reasons

ARAMammalPreload.m  -- create new species; I added the meta data information about the new species such as the Family; ToDO: add the descriptions, I didn't have all the details for the new ones

ARAReportViewController -- created a pList and added ALL the old and new locations. TODO: check for accuracy especially states such as Massachusetts which has three sub-areas - phone and state full name may be wrong. I don't know how the placemarks returns locations such as Massachusetts_Central? For the State full name, i used the same name as the .kml file name such as New_York instead of New York.

Is the "debug phone number" still necessary? I wasn't sure how to use it, so I included it in every state. It would be better to remove it so that the .pList is shorter. The original code includes one email address for all the states. I didn't change this although the .XLSX file has different email contacts for several locations.

Need help figuring out the relationship between the Washington locations - are these counties?? Need a polygon for the offshre islands? or add location coordinates?

Category.h and Category.m -- there seemed to be a problem with using the word "Category" - it's a reserved word, so I renamed the files NOAACategory.

ARACategoryListViewController -- TODO: change references from Category.h to ARACategory.h -- check this and other files for any reference to "Category"

TODO: DEPRECATED METHODS PROBLEM
UIAlertView -- the new way to do this is UIAlertController BUT the code that displays the alert is NSObject instead of a UIViewController, so we need a work around in order to present the UIAlertController. 

initWithPolygon - the replacement uses MKPloygonRenderer https://developer.apple.com/library/ios/documentation/MapKit/Reference/MKPolygonRenderer_clas/index.html#//apple_ref/occ/instm/MKPolygonRenderer/initWithPolygon:
this will require some fiddling around

