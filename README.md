# eth_abi_decoder PHP  BSC BINANCE SMART CHAIN

<?php

//download AND Extract zip file in vendor folder
// - -  https://github.com/kendol07/eth_abi_decoder

require __DIR__."/../../vendor/2amigos/ethereum-input-data-decoder-master/src/EthereumAbi.php";
require __DIR__."/../../vendor/2amigos/ethereum-input-data-decoder-master/src/InputDataDecoder.php";

$data = [
  "blockHash" => "0xfaa6ab98a791e6ef6cb70ebc9d611f074325b5550e0fae4972c2a8c1262c8ba7",
  "blockNumber" => "0x1b694c6",
  "from" => "0x392760369e0d81a156d7231a3fe177dba97dd22b",
  "gas" => "0x30d40",
  "gasPrice" => "0xb2d05e00",
  "hash" => "0x60c6ff9b16ddf2372cb7f8a1c02c990ae5c93162cf0bc8a866000a122dfba401",
  "input" => "0xa9059cbb00000000000000000000000065624442e8916b8cd4bc7c57388461bdc1bbe1a60000000000000000000000000000000000000000000000056bc75e2d63100000",
  "nonce" => "0x3ee",
  "to" => "0x55d398326f99059ff775485246999027b3197955",
  "transactionIndex" => "0x6f",
  "value" => "0x0",
  "type" => "0x0",
  "v" => "0x93",
  "r" => "0x1c59dfc1ab96126010300040e451375aaa13b15f86930df72e3fe09b2928a951",
  "s" => "0x44b25765a3268e457013ec144caa6532d476aae17f96a84449155527dfbdced1"
];

$inputData = $data['input'];
$abiArray = json_decode('[{"constant":true,"inputs":[],"name":"name","outputs":[{"name":"","type":"string"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_spender","type":"address"},{"name":"_value","type":"uint256"}],"name":"approve","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_pauseMaster","type":"address"}],"name":"setPauseMaster","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"totalSupply","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_from","type":"address"},{"name":"_to","type":"address"},{"name":"_value","type":"uint256"}],"name":"transferFrom","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"icoOpeningTime","outputs":[{"name":"","type":"uint64"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"decimals","outputs":[{"name":"","type":"uint8"}],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"withdraw","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"returnWei","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"value","type":"uint256"}],"name":"upgrade","outputs":[],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"closingTime","outputs":[{"name":"","type":"uint64"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"upgradeAgent","outputs":[{"name":"","type":"address"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"upgradeMaster","outputs":[{"name":"","type":"address"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_spender","type":"address"},{"name":"_subtractedValue","type":"uint256"}],"name":"decreaseApproval","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"_owner","type":"address"}],"name":"balanceOf","outputs":[{"name":"balance","type":"uint256"}],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"pause","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"owner","outputs":[{"name":"","type":"address"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"bounty","outputs":[{"name":"","type":"address"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"symbol","outputs":[{"name":"","type":"string"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_to","type":"address"},{"name":"_value","type":"uint256"}],"name":"transfer","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_upgradeAgent","type":"address"},{"name":"_revision","type":"uint32"}],"name":"setUpgradeAgent","outputs":[],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"phase","outputs":[{"name":"","type":"uint8"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_bounty","type":"address"}],"name":"setBounty","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"pauseMaster","outputs":[{"name":"","type":"address"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"totalUpgraded","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_spender","type":"address"},{"name":"_addedValue","type":"uint256"}],"name":"increaseApproval","outputs":[{"name":"success","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"pauseEnd","outputs":[{"name":"","type":"uint64"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"_owner","type":"address"},{"name":"_spender","type":"address"}],"name":"allowance","outputs":[{"name":"remaining","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"REVISION","outputs":[{"name":"","type":"uint32"}],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"create","outputs":[{"name":"success","type":"bool"}],"payable":true,"type":"function"},{"constant":true,"inputs":[],"name":"totalProceeds","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"newOwner","type":"address"}],"name":"transferOwnership","outputs":[],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"preIcoOpeningTime","outputs":[{"name":"","type":"uint64"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"returnAllowedTime","outputs":[{"name":"","type":"uint64"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"_upgradeMaster","type":"address"}],"name":"setUpgradeMaster","outputs":[],"payable":false,"type":"function"},{"inputs":[{"name":"_preIcoOpeningTime","type":"uint64"}],"payable":true,"type":"constructor"},{"payable":true,"type":"fallback"},{"anonymous":false,"inputs":[{"indexed":false,"name":"amount","type":"uint256"}],"name":"NewTokens","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"funder","type":"address"},{"indexed":false,"name":"value","type":"uint256"}],"name":"NewFunds","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"phase","type":"uint8"}],"name":"NewPhase","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"drawer","type":"address"},{"indexed":false,"name":"weiAmount","type":"uint256"}],"name":"Withdrawal","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"drawer","type":"address"},{"indexed":false,"name":"weiAmount","type":"uint256"}],"name":"Withdrawn","type":"event"},{"anonymous":false,"inputs":[],"name":"Paused","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"_from","type":"address"},{"indexed":false,"name":"_value","type":"uint256"}],"name":"Upgrade","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"agent","type":"address"}],"name":"UpgradeEnabled","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"previousOwner","type":"address"},{"indexed":true,"name":"newOwner","type":"address"}],"name":"OwnershipTransferred","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"owner","type":"address"},{"indexed":true,"name":"spender","type":"address"},{"indexed":false,"name":"value","type":"uint256"}],"name":"Approval","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"from","type":"address"},{"indexed":true,"name":"to","type":"address"},{"indexed":false,"name":"value","type":"uint256"}],"name":"Transfer","type":"event"}]');


$decoder = new \TWOamigos\InputDataDecoder($abiArray);
$decoded = $decoder->decodeData($inputData);
$encode = json_encode($decoded, true);
$decode = json_decode($encode, true);

$tokenDecimal=18;       //USDT 18 decimal
$contract=$data['to']; //USDT contract Token

$address = str_replace('000000000000000000000000', '0x', $decode['inputs'][0]); //address to
$decimals = '1' . str_repeat('0', $tokenDecimal); // Number of decimal places for the currency 18 = 1000000000000000000
$amount = hexdec($decode['inputs'][1]) / $decimals; //amount

// echo 'Type: ' . $decode['name'] . '<br>';

