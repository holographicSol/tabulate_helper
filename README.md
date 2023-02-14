# tabulate_helper


Compliment tabulate module.
Overcome potential Terminal/Console buffer limitations causing a table to not be entirely displayed.
Display N rows of table at a time, with some customization.


Simple Example:
tabulate_helper.display_rows_interactively(max_limit=75,
                                           results=_results,
                                           table=table_1,
                                           extra_input=False,
                                           message='\n--- more ---\n',
                                           function=None)
                                           

Note: Simply display rows until max_limit reached and display message.


Advanced Example:
tabulate_helper.display_rows_interactively(max_limit=75,
                                           results=a_list,
                                           table=a_table,
                                           extra_input=True,
                                           message='\n--- more ---\n',
                                           function=a_module.a_function_that_takes_input)


Note: a_function_that_takes_input may simply take digits that point at an index in results and
do something.
