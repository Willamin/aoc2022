# Day 1: Calorie Counting

## Part 1

```elixir
# from https://github.com/miladamilli/Advent_of_Code_2021
defmodule Load do
  def input do
    Path.join(__DIR__, "/../inputs/day01-input.txt")
    |> File.read!()
  end
end

Load.input()
```

<!-- livebook:{"output":true} -->

```
"4920\n3254\n4147\n1193\n6516\n4361\n7068\n2021\n\n5147\n3535\n5087\n3676\n2012\n5515\n3254\n6597\n1571\n4836\n2302\n5546\n5926\n\n33932\n34239\n\n2989\n2837\n7396\n1093\n2634\n1270\n5592\n5228\n3083\n5264\n6445\n2625\n\n5939\n1245\n4147\n4351\n2047\n2433\n2041\n6812\n5043\n1363\n3471\n2099\n4456\n\n5249\n5322\n1297\n6462\n3596\n5742\n4119\n4856\n4419\n4071\n1881\n5903\n2574\n\n1983\n10553\n10555\n\n2443\n3676\n8079\n2691\n6848\n4439\n6587\n4672\n5953\n1978\n2141\n\n6699\n8038\n1545\n8160\n2361\n1513\n2444\n2635\n\n2193\n10187\n1997\n7141\n2982\n8262\n3156\n6427\n\n3291\n11556\n8033\n6924\n4059\n11793\n\n4241\n7720\n11519\n1930\n1659\n4582\n\n1167\n7765\n1452\n5466\n2916\n7414\n7644\n7578\n7782\n8510\n\n2055\n4368\n8859\n7446\n4466\n6374\n8121\n4476\n\n19642\n\n19756\n5503\n14960\n\n4799\n5211\n4360\n1295\n3856\n6242\n3197\n6332\n1329\n2584\n6941\n4153\n\n4130\n3289\n9140\n10120\n9562\n2483\n3198\n1540\n\n3764\n6195\n3962\n2765\n3811\n6694\n5667\n1709\n1007\n2703\n3485\n5100\n\n4352\n10564\n2729\n13578\n8897\n1396\n\n1865\n3363\n9827\n5101\n10333\n10859\n9143\n\n4576\n5370\n5898\n3229\n6016\n2574\n6930\n1579\n4669\n4410\n5337\n3386\n4421\n\n13015\n\n1013\n4228\n4247\n7369\n1096\n1950\n1494\n8525\n5925\n\n5823\n10568\n5268\n5641\n8785\n8912\n11094\n\n3701\n7367\n4385\n1044\n6149\n5902\n6205\n5365\n3754\n5535\n1966\n\n4156\n3499\n1315\n6321\n6612\n6275\n5276\n2117\n1091\n6259\n5949\n1402\n5676\n\n2666\n3431\n1510\n1538\n5468\n5875\n2070\n2420\n6821\n5849\n4449\n5432\n\n9337\n9238\n10464\n18552\n\n1056\n1365\n4071\n6581\n8270\n8159\n4364\n10736\n\n13028\n5826\n15980\n1732\n\n4907\n1882\n2683\n4719\n6456\n4857\n3197\n3984\n6449\n1717\n3283\n2715\n2252\n5069\n\n7361\n1862\n2943\n4939\n5375\n3804\n4085\n5671\n1140\n6735\n7910\n\n5454\n7196\n3747\n7054\n6389\n5787\n3422\n8084\n\n1198\n5173\n4483\n5275\n3420\n4796\n1514\n3205\n5510\n4683\n3785\n4222\n2131\n4425\n1931\n\n2594\n5933\n1319\n2874\n4539\n1193\n5652\n3871\n2600\n4212\n2348\n2111\n3311\n1681\n5117\n\n6937\n17934\n17547\n2205\n\n42207\n\n6720\n6831\n6117\n2506\n6390\n4117\n4812\n3119\n1987\n4894\n6729\n2925\n\n1550\n4970\n9656\n2906\n4751\n4784\n3288\n1539\n6215\n\n13027\n7811\n\n13850\n10753\n9981\n6324\n8115\n5881\n\n2785\n3097\n5700\n7471\n2245\n1150\n4556\n4785\n4330\n1712\n2390\n\n7365\n10126\n10230\n1976\n9301\n3661\n4866\n3911\n\n9208\n4236\n\n5215\n4476\n1319\n6105\n2743\n1735\n1610\n4354\n5339\n4826\n1489\n2898\n1072\n3521\n4336\n\n4177\n2762\n2087\n6521\n6893\n3577\n7723\n2294\n2385\n6868\n1147\n\n7065\n4183\n5277\n6239\n4471\n1189\n2783\n5953\n2786\n4267\n\n7666\n6953\n1481\n3649\n1268\n3699\n6362\n8463\n\n1434\n3282\n2479\n4298\n6695\n5707\n4198\n5617\n4400\n2994\n6123\n3441\n3812\n\n1111\n5657\n1365\n1757\n6355\n1177\n8456\n\n11258\n16273\n11668\n\n9867\n4242\n3920\n16447\n\n4729\n2607\n6532\n18556\n\n4987\n1410\n2881\n1961\n4058\n6807\n8387\n7758\n8795\n1634\n\n5811\n3892\n1859\n5744\n7245\n7066\n7375\n1742\n5995\n4319\n2355\n7222\n\n30020\n4029\n\n2245\n10974\n15372\n11623\n8432\n\n5880\n1996\n1971\n7875\n2174\n2978\n1786\n8332\n4276\n6803\n\n8215\n6053\n8517\n2425\n1812\n2557\n10348\n10246\n\n8700\n4591\n5793\n5434\n1458\n6606\n5761\n1648\n5021\n4404\n\n3989\n2400\n7776\n7197\n7806\n10582\n5900\n2718\n\n6068\n1539\n3141\n1477\n1361\n2208\n5090\n1580\n5947\n5951\n1812\n5378\n5804\n5638\n5312\n\n4474\n\n6360\n4525\n4855\n5021\n2959\n2477\n1713\n4434\n5802\n2204\n3335\n4492\n5826\n1206\n\n7145\n13093\n1498\n3252\n15314\n\n15174\n16365\n10100\n16604\n\n4036\n2335\n1372\n1133\n2751\n3091\n6276\n5167\n3319\n4853\n4026\n2350\n3211\n6027\n\n11739\n7968\n6276\n8105\n3422\n11562\n8058\n\n2984\n3205\n5476\n4377\n2200\n1591\n2800\n4601\n1739\n1870\n4023\n5599\n4632\n3303\n3697\n\n4576\n9316\n10427\n7702\n9754\n7615\n9315\n4370\n\n2000\n1421\n2054\n2815\n5331\n7931\n2738\n5269\n2244\n6796\n\n6883\n6480\n3511\n3224\n5486\n2885\n3548\n3682\n4470\n3239\n4827\n\n7184\n9580\n1999\n5737\n4811\n8568\n4239\n8467\n4792\n\n5675\n1990\n\n7726\n7866\n7754\n4629\n2569\n1105\n3469\n2908\n4192\n1816\n\n2930\n\n6502\n4540\n7235\n1575\n1751\n3699\n2286\n3611\n2691\n6626\n5485\n\n3321\n2330\n7310\n6679\n4025\n4145\n9370\n6441\n1327\n\n24773\n14248\n13194\n\n9446\n3038\n2831\n8834\n10732\n6122\n4841\n\n4822\n7182\n5859\n5728\n6185\n4275\n1019\n6577\n5643\n3033\n\n5994\n2414\n3017\n5058\n1935\n1636\n1966\n4632\n5037\n5616\n4686\n4674\n\n3106\n3734\n5023\n6156\n1402\n3712\n5019\n2790\n5008\n1117\n4757\n6008\n6083\n6105\n\n4042\n7107\n4882\n6935\n1690\n4427\n2346\n2091\n4643\n7097\n1904\n7194\n\n7018\n9025\n8470\n1859\n6322\n2228\n4829\n8897\n3612\n\n4117\n1656\n4928\n1508\n2667\n5532\n3710\n1773\n2931\n3233\n5294\n4164\n3833\n3720\n\n3205\n4498\n2911\n2405\n3073\n3954\n2897\n1747\n6012\n3894\n1809\n2322\n3037\n5080\n5642\n\n3140\n5499\n5095\n6787\n3287\n3524\n4932\n4821\n1057\n4864\n6707\n7472\n\n5519\n3772\n1426\n4295\n2918\n7749\n5899\n7046\n5555\n2867\n1064\n\n1971\n3997\n5732\n4127\n4844\n2388\n1309\n4246\n2785\n4623\n5799\n1165\n6172\n4262\n\n131" <> ...
```

Santa's reindeer typically eat regular reindeer food, but they need a lot of magical energy to deliver presents on Christmas. For that, their favorite snack is a special type of star fruit that only grows deep in the jungle. The Elves have brought you on their annual expedition to the grove where the fruit grows.

To supply enough magical energy, the expedition needs to retrieve a minimum of fifty stars by December 25th. Although the Elves assure you that the grove has plenty of fruit, you decide to grab any fruit you see along the way, just in case.

Collect stars by solving puzzles. Two puzzles will be made available on each day in the Advent calendar; the second puzzle is unlocked when you complete the first. Each puzzle grants one star. Good luck!

The jungle must be too overgrown and difficult to navigate in vehicles or access from the air; the Elves' expedition traditionally goes on foot. As your boats approach land, the Elves begin taking inventory of their supplies. One important consideration is food - in particular, the number of Calories each Elf is carrying (your puzzle input).

The Elves take turns writing down the number of Calories contained by the various meals, snacks, rations, etc. that they've brought with them, one item per line. Each Elf separates their own inventory from the previous Elf's inventory (if any) by a blank line.

For example, suppose the Elves finish writing their items' Calories and end up with the following list:

```elixir
sample = """
1000
2000
3000

4000

5000
6000

7000
8000
9000

10000
"""
```

<!-- livebook:{"output":true} -->

```
"1000\n2000\n3000\n\n4000\n\n5000\n6000\n\n7000\n8000\n9000\n\n10000\n"
```

This list represents the Calories of the food carried by five Elves:

The first Elf is carrying food with `1000`, `2000`, and `3000` Calories, a total of `6000` Calories.
The second Elf is carrying one food item with `4000` Calories.
The third Elf is carrying food with `5000` and `6000` Calories, a total of `11000` Calories.
The fourth Elf is carrying food with `7000`, `8000`, and `9000` Calories, a total of `24000` Calories.
The fifth Elf is carrying one food item with `10000` Calories.
In case the Elves get hungry and need extra snacks, they need to know which Elf to ask: they'd like to know how many Calories are being carried by the Elf carrying the **most** Calories. In the example above, this is `24000` (carried by the fourth Elf).

Find the Elf carrying the most Calories. How many total Calories is that Elf carrying?

```elixir
defmodule Part1 do
  def total_of_max(input) do
    input
    |> String.split("\n")
    |> Enum.map(fn s ->
      case Integer.parse(s) do
        {i, _} -> i
        _ -> nil
      end
    end)
    |> Enum.chunk_by(fn x -> x == nil end)
    |> Enum.reject(fn x -> x == [nil] end)
    |> Enum.map(fn list ->
      list |> Enum.reduce(fn x, acc -> x + acc end)
    end)
    |> Enum.sort()
    |> Enum.reverse()
    |> hd()
  end
end

Part1.total_of_max(sample)
```

<!-- livebook:{"output":true} -->

```
24000
```

## Part 2

By the time you calculate the answer to the Elves' question, they've already realized that the Elf carrying the most Calories of food might eventually run out of snacks.

To avoid this unacceptable situation, the Elves would instead like to know the total Calories carried by the top three Elves carrying the most Calories. That way, even if one of those Elves runs out of snacks, they still have two backups.

In the example above, the top three Elves are the fourth Elf (with `24000` Calories), then the third Elf (with `11000` Calories), then the fifth Elf (with `10000` Calories). The sum of the Calories carried by these three elves is `45000`.

Find the top three Elves carrying the most Calories. How many Calories are those Elves carrying in total?

```elixir
defmodule Part2 do
  def total_of_top_three(input) do
    input
    |> String.split("\n")
    |> Enum.map(fn s ->
      case Integer.parse(s) do
        {i, _} -> i
        _ -> nil
      end
    end)
    |> Enum.chunk_by(fn x -> x == nil end)
    |> Enum.reject(fn x -> x == [nil] end)
    |> Enum.map(fn list ->
      Enum.sum(list)
    end)
    |> Enum.sort()
    |> Enum.reverse()
    |> Enum.take(3)
    |> Enum.sum()
  end
end

Part2.total_of_top_three(sample)
```

<!-- livebook:{"output":true} -->

```
45000
```

## Final Outputs

```elixir
%{part1: Part1.total_of_max(Load.input()), part2: Part2.total_of_top_three(Load.input())}
```

<!-- livebook:{"output":true} -->

```
%{part1: 69177, part2: 207456}
```

## Refactoring

```elixir
defmodule Refactor do
  def total_of_max(input, elves_considered) do
    input
    |> String.split("\n\n")
    |> Enum.map(fn a ->
      a
      |> String.split("\n")
      |> Enum.flat_map(fn s ->
        case Integer.parse(s) do
          {i, _} -> [i]
          _ -> []
        end
      end)
      |> Enum.sum()
    end)
    |> Enum.sort()
    |> Enum.reverse()
    |> Enum.take(elves_considered)
    |> Enum.sum()
  end
end

%{
  part1: %{
    original_code: Part1.total_of_max(Load.input()),
    refactored: Refactor.total_of_max(Load.input(), 1)
  },
  part2: %{
    original_code: Part2.total_of_top_three(Load.input()),
    refactored: Refactor.total_of_max(Load.input(), 3)
  }
}
```

<!-- livebook:{"output":true} -->

```
%{
  part1: %{original_code: 69177, refactored: 69177},
  part2: %{original_code: 207456, refactored: 207456}
}
```
