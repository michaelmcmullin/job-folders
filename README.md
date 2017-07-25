# Job Folders
A handy little AppleScript for creating predefined folder structures. Out of the box,
its use is pretty specialised, as it was created for how we handle jobs in our work.
However, it's easy enough to adapt to other needs.

## Current structure
In our company, each job has a unique number (say, 123456). All files relating to that
job should be placed in a folder named with the job number and customer name. Within
this folder, there are three sub-folders (PRINT, Art, Source Files):

    123456.Apple Inc
    - Art
    - PRINT
    - Source Files

If a job has multiple parts, things get a little more complex. Within the main job
folder, each part has another folder that follows the structure above. However, each
part is named after the job number, followed by a 2-digit part number:

    123456.Apple Inc
    - 123456.01
      - Art
      - PRINT
      - Source Files
    - 123456.02
      - Art
      - PRINT
      - Source Files
    - 123456.03
      - Art
      - PRINT
      - Source Files

Creating this structure manually is time consuming. Instead, this script presents
the user with a dialog box for the job number, customer, and number of parts. Job
done!
