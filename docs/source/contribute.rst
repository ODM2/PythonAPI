Contributing
============================

You can help with ODM2 Python API by contributing code, helping with the documentation, or engaging the team via `GitHub issues <https://github.com/ODM2/ODM2PythonAPI/issues>`_ (questions, solutions, etc).


Install the development version from GitHub
--------------------------------------------

The latest development version is found in the ``development`` branch of the github repository. We follow the `Gitflow workflow <https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow>`__ for development.

1. Download both ``requirements.txt`` and ``requirements-dev.txt``.

   .. code-block:: bash

       wget https://raw.githubusercontent.com/ODM2/ODM2PythonAPI/master/requirements.txt
       wget https://raw.githubusercontent.com/ODM2/ODM2PythonAPI/master/requirements-dev.txt

2. Create conda environment ``odm2api_dev`` from the two ``requirements*`` text files.

   .. code-block:: bash

       conda create -n odm2api_dev -c conda-forge python=2.7 --file requirements.txt --file requirements-dev.txt

3. Activate conda environment.
   - MacOSX/Linux:

   .. code-block:: bash

       source activate odm2api_dev

   - Windows:

   .. code-block:: bash

       activate odm2api_dev

4. Install the latest commit from the development branch

   .. code-block:: bash

       pip install git+https://github.com/ODM2/ODM2PythonAPI.git@development#egg=odm2api


Contribute to documentation
----------------------------------

This guide is a reference on how to contribute to ODM2 Documentation effort
for the many `ODM2 Software Ecosystem <https://github.com/ODM2/odm2-software-ecosystem>`__.

Conventions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

There are a few conventions that should be followed
when writing docstrings within the code:

- Docstrings should follow
  `Google Style Documentation
  <http://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html>`__.

- Do not say "**defaults to ____**" for any arguments,
  unless the argument needs further explanation.
  The default value is already available in the method/function definition.

- If function needs to be instantiated, explicitly show in example.
  See
  `here <https://stackoverflow.com/questions/17134653/difference-between-class-and-instance-methods>`__
  for discussion of class vs instance methods.

- Provide link to `Controlled Vocabulary <http://vocabulary.odm2.org/>`__
  if an argument needs a CV as value.

Please add any additional conventions that you think should be in place
within `the github issue #106 <https://github.com/ODM2/ODM2PythonAPI/issues/106>`__.

Pull requests
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Once changes has been in place within your forked copy of the repository
you are working on, please create a pull request to add your contribution
to the **development** branch of the repository.
