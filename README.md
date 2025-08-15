# LeetCode Problems — JSON Dataset

This repository provides a dataset of LeetCode problems in JSON format. Each problem is saved as a separate `.json` file within the `problems/` directory, and all problems are also combined in a single `merged_problems.json` file for easy access.

## Dataset Structure

- `problems/`: Contains individual LeetCode problems as separate `.json` files. Each file is named with the problem's ID and a slug (e.g., `0001-two-sum.json`).
- `merged_problems.json`: A single file containing all problems merged into a list.

## Updated JSON Schema for Each Problem

Each problem JSON file contains the following fields:

- `title`: The name of the problem (e.g., "Container With Most Water").
- `problem_id`: The internal problem ID (string).
- `frontend_id`: The LeetCode frontend ID (string).
- `difficulty`: The difficulty level (`Easy`, `Medium`, or `Hard`).
- `problem_slug`: The URL-friendly name (e.g., `container-with-most-water`).
- `topics`: Array of topic tags (e.g., `Array`, `Two Pointers`).
- `description`: The full problem statement, usually in Markdown format.
- `examples`: Array of example objects, each with:
    - `example_num`: Example number
    - `example_text`: Input/output and explanation
    - `images`: Array of image URLs (if available)
- `constraints`: Array of constraints or limits for the problem.
- `follow_ups`: Array of follow-up questions (if any).
- `hints`: Array of hints for solving the problem.
- `code_snippets`: Object containing starter code for various languages (e.g., `python`, `cpp`, `java`, etc.)
- `solutions`: HTML string containing editorial content for some problems.

## Example Problem JSON

```json
{
  "title": "Container With Most Water",
  "problem_id": "11",
  "frontend_id": "11",
  "difficulty": "Medium",
  "problem_slug": "container-with-most-water",
  "topics": [
      "Array",
      "Two Pointers",
      "Greedy"
  ],
  "description": "You are given an integer array height of length n...",
  "examples": [
    {
      "example_num": 1,
      "example_text": "Input: height = [1,8,6,2,5,4,8,3,7]\\nOutput: 49\\nExplanation: ...",
      "images": ["https://s3-lc-upload.s3.amazonaws.com/uploads/2018/07/17/question_11.jpg"]
    },
    {
      "example_num": 2,
      "example_text": "Input: height = [1,1]\\nOutput: 1",
      "images": ["https://s3-lc-upload.s3.amazonaws.com/uploads/2018/07/17/question_11.jpg"]
    }
  ],
  "constraints": [
    "n == height.length",
    "2 <= n <= 105",
    "0 <= height[i] <= 104"
  ],
  "follow_ups": [],
  "hints": [
    "If you simulate the problem, it will be O(n^2) which is not efficient.",
    "Try to use two-pointers...",
    "How can you calculate the amount of water at each step?"
  ],
  "code_snippets": {
    "cpp": "class Solution {\npublic:\n    int maxArea(vector<int>& height) {\n        \n    }\n};",
    "java": "class Solution {\n    public int maxArea(int[] height) {\n        \n    }\n}",
    "python": "class Solution(object):\n    def maxArea(self, height):\n        \"\"\"\n        :type height: List[int]\n        :rtype: int\n        \"\"\"\n        ",
    "python3": "class Solution:\n    def maxArea(self, height: List[int]) -> int:\n        ",
    "c": "int maxArea(int* height, int heightSize) {\n    \n}",
    "csharp": "public class Solution {\n    public int MaxArea(int[] height) {\n        \n    }\n}",
    "javascript": "/**\n * @param {number[]} height\n * @return {number}\n */\nvar maxArea = function(height) {\n    \n};",
    "typescript": "function maxArea(height: number[]): number {\n    \n};",
    "php": "class Solution {\n\n    /**\n     * @param Integer[] $height\n     * @return Integer\n     */\n    function maxArea($height) {\n        \n    }\n}",
    "swift": "class Solution {\n    func maxArea(_ height: [Int]) -> Int {\n        \n    }\n}",
    "kotlin": "class Solution {\n    fun maxArea(height: IntArray): Int {\n        \n    }\n}",
    "dart": "class Solution {\n  int maxArea(List<int> height) {\n    \n  }\n}",
    "golang": "func maxArea(height []int) int {\n    \n}",
    "ruby": "# @param {Integer[]} height\n# @return {Integer}\ndef max_area(height)\n    \nend",
    "scala": "object Solution {\n    def maxArea(height: Array[Int]): Int = {\n        \n    }\n}",
    "rust": "impl Solution {\n    pub fn max_area(height: Vec<i32>) -> i32 {\n        \n    }\n}",
    "racket": "(define/contract (max-area height)\n  (-> (listof exact-integer?) exact-integer?)\n  )",
    "erlang": "-spec max_area(Height :: [integer()]) -> integer().\nmax_area(Height) ->\n  .",
    "elixir": "defmodule Solution do\n  @spec max_area(height :: [integer]) :: integer\n  def max_area(height) do\n    \n  end\nend"
  }
}
```

## Notes
- Some fields (like `solutions`, `images`, `follow_ups`) may be missing for certain problems.

## Usage

You can use this dataset for:
- Building practice tools
- Analyzing problem trends
- Interview preparation
- Educational projects

Feel free to contribute or suggest improvements!
