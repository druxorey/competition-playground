
<h1 align="center">Competition Playground</h1>

<p align="center">
<a href="#repository-structure"><img src="https://img.shields.io/badge/structure-BD93F9?style=for-the-badge"></a>
<a href="#how-to-execute-scripts"><img src="https://img.shields.io/badge/how%20to%20run-BD93F9?style=for-the-badge"></a>
</p>

<p align="center">A repository for competitive programming exercises and their solutions in C++</p>

## Repository Structure

- **Exercises**: Each exercise is stored in its own directory. The structure of each directory is as follows:
  - `exercise.md`: Contains the problem statement in Markdown format.
  - `main.cpp`: Contains the solution code for the exercise.
  - `test.cpp`: Contains test cases for the solution, written using the `doctest.h` testing framework.

## How To Execute Scripts

### Compiling and Running `main.cpp`

To compile and run the solution code (`main.cpp`), navigate to the directory containing the exercise and use the following commands:

```bash
g++ main.cpp -o main
./main
```

### Compiling and Running `test.cpp`

To compile and run the test cases (`test.cpp`), ensure that the `doctest.h` header file is available in the same directory or in your include path. Then, use the following commands:

```bash
g++ test.cpp -o test
./test
```

## Contribute

If you want to add new exercises or improve existing ones, follow these steps:

1. Open an issue to discuss the changes.
2. Fork this repository.
3. Create a new branch for your contribution: `git checkout -b your-branch-name`.
4. Make your changes. To add new exercises, create a new directory for the exercise and include the `exercise.md`, `main.cpp`, and `test.cpp` files.
5. Commit your changes, for example: `git commit -m 'feat(exercises): added new exercise "binary-search"'`.
6. Push your changes to your forked repository: `git push origin your-branch-name`.
7. Open a Pull Request in this repository and reference the original issue.

## License

This project is licensed under the GPL-3.0 License. See the [LICENSE](LICENSE) file for more details.
