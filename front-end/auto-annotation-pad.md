## S1: Auto Annotation - Normal Flow 1 
Visit the auto annotate page, clear the input number '0' and enter '50'. Visit the task panel to see whether there is a task and stop it. Enter '5' to see whether there are 5 images in Annotated Data page.
1. Go to `Auto Annotate` page, set the number to be 50, and start auto annotation. Task center component should now have 1 task in it.
2. Wait for 10 seconds, stop the task center. There should be a text suggest "No task is running now."
3. Go to `Auto Annotate` page, set the number to be 5, and start auto annotation. Task center component should now have 1 task in it(Actual: Could not find element: [data-test=task-panel-item-name])
4. Wait for 10 seconds, the task center should be empty.(Actual: There are many delayed tasks)
5. Go back to `Annotated` page. There should be 5 images in it. (Actual: There are 8 images in it)
